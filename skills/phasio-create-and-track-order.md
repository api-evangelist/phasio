---
name: Create and track a Phasio manufacturing order
description: Authenticate to the Phasio Manufacturer API, create an order, validate part manufacturability, and monitor it through the Kanban production board.
api: openapi/phasio-openapi-original.json
operations: [create_10, getById_2, validatePartManufacturabilityForOrder, updateKanbanColumn, get_7]
---

# Create and track a Phasio manufacturing order

Operating instructions for using the Phasio Manufacturer API v1
(`https://m-api.eu.phas.io/api/manufacturer/v1`) to place and track a
manufacturing order. All operationIds below are verified against
`openapi/phasio-openapi-original.json`.

## Authenticate
1. Obtain a Bearer token via OAuth 2.0 client-credentials at
   `https://auth.eu.phas.io/oauth2/token` (client_id/client_secret created under
   Settings > API Keys in the manufacturer dashboard).
2. Send `Authorization: Bearer <access_token>` on every request. Tokens are JWTs.

## Steps
1. **Create the order** — `POST /order` (`create_10`). Supply the order body.
   For safe retries on network failures, send an `Idempotency-Key` header where
   supported (see `conventions/phasio-conventions.yml`).
2. **Fetch it back** — `GET /order/{id}` (`getById_2`) to read the created order,
   its requisitions (per-part line items), and shipment.
3. **Validate manufacturability** — `GET /order/{id}/manufacturability`
   (`validatePartManufacturabilityForOrder`) before committing to production.
4. **Advance production** — `PATCH /order/{id}/kanban-column`
   (`updateKanbanColumn`) to move the order across the production Kanban board.
5. **Poll the queue** — `GET /order` (`get_7`) with an RSQL `filter` (e.g.
   `paymentStatus=in=(PAID,UNPAID)`), `search`, `sort`, `page`, `size` to list
   and reconcile orders.

## Conventions and errors
- Pagination is page-number style; responses carry `content` + `totalElements` +
  `totalPages` + paging flags.
- Errors are returned as `application/json` with standard HTTP status codes
  (400/401/403/404/409/429/500/503) — see `errors/phasio-problem-types.yml`.
- On `429`, back off and retry.
