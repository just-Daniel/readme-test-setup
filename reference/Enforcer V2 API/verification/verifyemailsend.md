---
title: Send email verification OTP
excerpt: >-
  Sends a 6-digit OTP to the user's email address for verification. If the user
  has no email on file, the email field is required and will be set on the
  account. Admins and tenant admins can specify a user_id to trigger
  verification for another user.
api:
  file: openapi.json
  operationId: verifyEmailSend
hidden: false
---