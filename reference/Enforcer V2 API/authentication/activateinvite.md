---
title: Activate an invited user account
excerpt: >-
  Activates an inactive user account using a tenant secret. Supports two modes:

  **Privy mode** (when Privy auth is configured): Provide a Bearer {privy_token}
  in the Authorization header. The user is identified by their Privy DID.

  **Non-Privy mode** (when Privy auth is NOT configured): Provide the user's
  email in the request body. The user is identified by their email address.
api:
  file: openapi.json
  operationId: activateInvite
hidden: false
---