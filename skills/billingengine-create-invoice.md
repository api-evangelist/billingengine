---
name: billingengine-create-invoice
description: Create a draft invoice, retrieve it, and download its PDF representation.
api: openapi/billingengine-openapi.json
operations:
- createInvoice
- getInvoice
- downloadInvoicePdf
generated: '2026-10-19'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/billingengine-openapi.json ; every operationId checked against the contract
---

# billingengine-create-invoice

Create a draft invoice, retrieve it, and download its PDF representation.

## Steps

1. 1. Call `createInvoice` with the required request body fields for a draft invoice.
2. 2. Call `getInvoice` with the `id` returned from `createInvoice` to verify the invoice details.
3. 3. Call `downloadInvoicePdf` with the same `id` to obtain the invoice PDF.

## Rules

- All requests must include an `Authorization: Bearer <token>` header (bearerAuth).
- The `listInvoices` operation supports pagination via `page` and `pageSize` query parameters (if used).
