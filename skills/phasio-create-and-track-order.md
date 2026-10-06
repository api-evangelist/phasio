---
name: Create and track a Phasio manufacturing order
description: Authenticate to the Phasio Manufacturer API, create an order, and monitor it through the Kanban production board.
api: openapi/_original/phasio-openapi.json
operations: [create_2, getById_5, updateKanbanColumn, get_2]
---

# Create and track a Phasio manufacturing order

Operating instructions for using the Phasio Manufacturer API v1
(`https://m-api.eu.phas.io/api/manufacturer/v1`) to place and track a
manufacturing order. All operationIds below are verified against
`openapi/_original/phasio-openapi.json` (current contract, 2026-10-06).

## Authenticate
1. Create an API key under Settings > API Keys in the manufacturer dashboard.
2. Send it as `Authorization: Bearer <api_key>` on every request.

## Steps
1. **Create the order** — `POST /order` (`create_2`). Supply the order body.
   For safe retries on network failures, send an `Idempotency-Key` header where
   supported (see `conventions/phasio-conventions.yml`).
2. **Fetch it back** — `GET /order/{id}` (`getById_5`) to read the created order,
   its requisitions (per-part line items), and shipping.
3. **Advance production** — `PATCH /order/{id}/kanban-column`
   (`updateKanbanColumn`) to move the order across the production Kanban board.
4. **Poll the queue** — `GET /order` (`get_2`) with an RSQL `filter` (e.g.
   `paymentStatus=in=(PAID,UNPAID)`), `search`, `sort`, `page`, `size` to list
   and reconcile orders.

## Conventions and errors
- Pagination is page-number style; responses carry `content` + `totalElements` +
  `totalPages` + paging flags.
- Errors are returned as `application/json` with standard HTTP status codes
  (400/401/403/404/409/429/500/503) — see `errors/phasio-problem-types.yml`.
- On `429`, back off and retry.
