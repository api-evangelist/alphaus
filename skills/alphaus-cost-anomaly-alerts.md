---
name: Configure cost anomaly alerts
description: Create and manage cost anomaly alerts on registered cloud accounts using the Blue API Cover service.
api: openapi/alphaus-blueapi-openapi-original.json
operations: [Cover_RegisterDataAccess, Cover_CreateAnomalyAlert, Cover_ListAnomalyAlert, Cover_GetAnomalyAlert, Cover_DeleteAnomalyAlert]
---

# Configure cost anomaly alerts

The Cover service ingests cost/usage data and raises anomaly alerts.

## Steps

1. **Register data access** for an account with `Cover_RegisterDataAccess`
   (`POST /v1/account`) so Cover can read its cost and usage.
2. **Create an anomaly alert** with `Cover_CreateAnomalyAlert`
   (`POST /v1/alerts/anomaly`).
3. **List** existing anomaly alerts with `Cover_ListAnomalyAlert`
   (`POST /v1/alerts/anomaly/all:read`) and **fetch one** with `Cover_GetAnomalyAlert`
   (`GET /v1/alerts/anomaly/{id}`).
4. **Delete** an alert with `Cover_DeleteAnomalyAlert`
   (`DELETE /v1/alerts/anomaly/{id}`).

## Rules

- Bearer-token auth; the caller needs RBAC permission on the Cover product.
- Register data access before creating alerts — alerts on an unregistered account
  fail with `FAILED_PRECONDITION`.
- List/read verbs are `POST .../:read` with the filter in the body.
