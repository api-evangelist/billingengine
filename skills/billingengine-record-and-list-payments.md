---
name: billingengine-record-and-list-payments
description: Record a new payment and then retrieve the list of payments.
api: openapi/billingengine-openapi.json
operations:
- createPayment
- listPayments
generated: '2026-10-19'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/billingengine-openapi.json ; every operationId checked against the contract
---

# billingengine-record-and-list-payments

Record a new payment and then retrieve the list of payments.

## Steps

1. 1. Use `createPayment` with the request body fields required to record a payment (fields not specified in the documentation).
2. 2. Use `listPayments` to retrieve the collection of payments.

## Rules

- Include an `Authorization: Bearer <token>` header as defined by the bearerAuth scheme.
