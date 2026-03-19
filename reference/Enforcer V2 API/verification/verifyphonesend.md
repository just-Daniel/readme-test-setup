---
title: Send phone verification OTP
excerpt: >-
  Sends a 6-digit OTP via SMS to the user's phone number for verification. If
  the user has no phone number on file, the phone_number field is required and
  will be set on the account. Admins and tenant admins can specify a user_id to
  trigger verification for another user.
api:
  file: openapi.json
  operationId: verifyPhoneSend
hidden: false
---