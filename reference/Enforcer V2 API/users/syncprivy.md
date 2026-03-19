---
title: Sync Privy wallet data
excerpt: >-
  Backfills wallet addresses from the user's Privy linked accounts into the
  local auth_providers table.

  Requires the request to be authenticated via a Privy-issued token. Skips if
  wallet data already exists unless force=true.
api:
  file: openapi.json
  operationId: syncPrivy
hidden: false
---