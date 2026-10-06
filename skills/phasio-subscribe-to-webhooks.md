---
name: Subscribe to Phasio order and quote webhooks
description: Register, list, and remove Phasio webhooks and verify signed, encrypted event payloads.
api: openapi/_original/phasio-openapi.json
operations: [createWebhook, getWebhooks, deleteWebhook]
---

# Subscribe to Phasio order and quote webhooks

Operating instructions for the Phasio webhook surface
(`/api/manufacturer/v1/webhook`). operationIds verified against
`openapi/_original/phasio-openapi.json`; event and signature details from
`asyncapi/phasio-webhooks.yml`.

## Authenticate
Use `Authorization: Bearer <api_key>` with an API key created under
Settings > API Keys in the manufacturer dashboard.

## Steps
1. **Register an endpoint** — `POST /webhook` (`createWebhook`) with an
   `https://` (public, non-private) URL and a trigger event type. Phasio returns
   a per-webhook Base64-encoded AES-256 secret.
2. **List endpoints** — `GET /webhook` (`getWebhooks`) to review registered
   webhooks.
3. **Remove an endpoint** — `DELETE /webhook/{id}` (`deleteWebhook`).

## Event types
`ORDER`, `ORDER_UPDATED`, `QUOTE_CONVERTED`, `CUSTOMER_ORGANISATION_CREATED`,
`CUSTOMER_ORGANISATION_UPDATED`, `SPECIFICATION_CREATED`, `CART_CREATED`.

## Verifying a delivery
- Payloads arrive as `Content-Type: application/json` with header
  `X-Phasio-Signature` = hex HMAC-SHA256 of the **encrypted** payload string.
- The body is AES-256-GCM encrypted (Base64 URL-safe). Base64-decode your secret
  to get the key, verify the HMAC over the encrypted string, then decrypt.
- Reject deliveries whose recomputed signature does not match.
