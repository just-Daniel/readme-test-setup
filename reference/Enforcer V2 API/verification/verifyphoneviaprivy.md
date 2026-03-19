---
title: Verify phone via Privy
excerpt: >-
  Fetches the user's Privy account by DID, extracts a verified phone number from
  their linked accounts (SMS login), writes it to the database, and marks
  phone_number_verified = true. Requires the user to have a linked Privy user
  ID. Admins and tenant admins can specify a user_id to verify another user.
api:
  file: openapi.json
  operationId: verifyPhoneViaPrivy
hidden: false
---