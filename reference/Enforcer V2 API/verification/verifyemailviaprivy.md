---
title: Verify email via Privy
excerpt: >-
  Fetches the user's Privy account by DID, extracts a verified email from their
  linked accounts, writes it to the database, and marks email_verified = true.
  Requires the user to have a linked Privy user ID. Admins and tenant admins can
  specify a user_id to verify another user.
api:
  file: openapi.json
  operationId: verifyEmailViaPrivy
hidden: false
---