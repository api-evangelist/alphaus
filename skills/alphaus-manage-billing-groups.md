---
name: Manage reseller billing and access groups
description: Create access groups and assign accounts to billing groups for reseller invoicing via the Blue API Billing service.
api: openapi/alphaus-blueapi-openapi-original.json
operations: [Billing_ListAccessGroups, Billing_CreateAccessGroup, Billing_AddAccountToBillingGroup, Billing_AddBillingGroupCustomField]
---

# Manage reseller billing and access groups

The Billing service (Ripple) organizes reseller customers into access groups and
billing groups for invoicing.

## Steps

1. **List access groups** with `Billing_ListAccessGroups` (`GET /v1/accessgroups`).
2. **Create an access group** with `Billing_CreateAccessGroup`
   (`POST /v1/accessgroups`).
3. **Assign a cloud account to a billing group** with
   `Billing_AddAccountToBillingGroup` (`POST /v1/billinggroup/account`).
4. **Attach a custom field** (e.g. cost-center) with
   `Billing_AddBillingGroupCustomField` (`POST /v1/billinggroup/customfield`).

## Rules

- Requires an OAuth2 bearer token with RBAC permission for reseller billing.
- `groupId` / `billingInternalId` reference an existing billing group — resolve it
  before assigning accounts.
- No idempotency key: check with a list call before re-creating a group to avoid
  `ALREADY_EXISTS` (409).
