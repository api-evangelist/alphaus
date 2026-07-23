---
name: Authenticate to Blue API and provision an API client
description: Obtain an OAuth2 access token for the Alphaus Blue API and create/list machine API clients via the Iam service.
api: openapi/alphaus-blueapi-openapi-original.json
operations: [Iam_CreateApiClient, Iam_ListApiClients, Iam_DeleteApiClient]
---

# Authenticate to Blue API and provision an API client

Blue API (`https://api.alphaus.cloud/m/blue`) authenticates with **OAuth2 client
credentials**. Fine-grained authorization is enforced by the Iam service (RBAC).

## Steps

1. **Mint an access token.** POST your client credentials to the token endpoint
   (Ripple/Octo: `https://login.alphaus.cloud/ripple/access_token`; WavePro:
   `https://login.alphaus.cloud/access_token`) with
   `grant_type=client_credentials` and `scope=openid`. Read `access_token` from
   the JSON response.
2. **Send the token on every call** as `Authorization: Bearer <access_token>`.
3. **List existing API clients** with `Iam_ListApiClients` (`GET /iam/v1/apiclients`).
4. **Create a new machine client** with `Iam_CreateApiClient`
   (`POST /iam/v1/apiclients`) — this returns the client id/secret used by the
   token exchange above.
5. **Revoke** a client you no longer need with `Iam_DeleteApiClient`
   (`DELETE /iam/v1/apiclients/{id}`).

## Rules

- Tokens expire (`expires_in`); refresh by re-running step 1. Do not hardcode tokens.
- Errors use the `google.rpc.Status` envelope (`code`, `message`, `details`) —
  `UNAUTHENTICATED` (401) means the token is missing/expired; `PERMISSION_DENIED`
  (403) means the caller lacks the RBAC permission.
- No idempotency-key header is supported; retries of create calls may create duplicates.
