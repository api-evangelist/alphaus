---
name: Query and export cloud costs
description: Read invoice costs and export cost reports across AWS/Azure/GCP accounts using the Blue API Cost service.
api: openapi/alphaus-blueapi-openapi-original.json
operations: [Cost_ListAccounts, Cost_ReadInvoiceCosts, Cost_ReadInvoiceGroupCosts, Cost_ExportReport]
---

# Query and export cloud costs

The Cost service exposes multi-cloud cost data. Operations that take a `{vendor}`
path segment accept `aws`, `azure`, or `gcp`.

## Steps

1. **List the accounts** you can see for a vendor with `Cost_ListAccounts`
   (`GET /v1/{vendor}/accounts`).
2. **Read invoice costs** with `Cost_ReadInvoiceCosts` (`POST /v1/invoicecosts:read`),
   or aggregate by billing group with `Cost_ReadInvoiceGroupCosts`
   (`POST /v1/invoicegroupcosts:read`). These are `:read` verbs — the query body
   carries the filters (period, grouping).
3. **Export a full report** with `Cost_ExportReport` (`POST /v1/reports:export`).

## Rules

- Send `Authorization: Bearer <token>` on every request (see the authenticate skill).
- Read-style queries are modeled as `POST .../:read` because the filter payload is
  large — put filters in the request body, not query params.
- `:read`/`:export` responses can be large and server-streamed; handle chunked results.
- Errors surface as `google.rpc.Status`; `INVALID_ARGUMENT` (400) usually means a
  malformed period or unknown vendor.
