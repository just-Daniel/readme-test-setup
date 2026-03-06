---
title: Transfer Apple SK2 purchase
excerpt: >-
  Use this endpoint to transfer an existing **active** purchase from one user to
  another. This allows re-assigning access to a subscription or in-app
  purchase.  <br><br> The transfer process is asynchronous. Upon successful
  registration, the API will return a `202` `Accepted` status with a unique
  `synchronizationId` in the response body. <br><br> **Note:** Only active
  purchases can be transferred.  <br><br>Please note that **this endpoint can be
  authorized with a publisher (X-Publisher-Token) or JWT (Bearer) token**.
  Depending on how you integrate with Cleeng (directly or through middleware),
  use either a <<glossary:JWT>> or X-Publisher-Token header authorization. <br>
  <br> <span style="color:green">**Please use JWT (Bearer) token to try out the
  endpoint in the API console in this documentation**.</span>
api:
  file: test.json
  operationId: transfer-apple-sk2-purchase
hidden: false
---