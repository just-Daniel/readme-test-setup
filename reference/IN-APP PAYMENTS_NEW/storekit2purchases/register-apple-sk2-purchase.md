---
title: Register Apple SK2 purchase
excerpt: >-
  Use this endpoint to register a purchase made via Apple StoreKit2 to initiate
  an asynchronous  synchronization process. This process involves verifying the
  purchase with Apple and updating the user's entitlement status in Cleeng's
  system. <br><br> Due to the time required for Apple's verification, this
  operation is asynchronous. Upon successful registration, the API will return a
  `202` `Accepted` status with a unique `synchronizationId` in the response
  body. <br><br> The `cleengCustomerId` is used to identify the user in Cleeng's
  system and associate the purchase with their account. <br><br> **Important:**
  Only one synchronization process can be active for a given `transactionId` at
  a time. If a new request is made for the same `transactionId` while a previous
  synchronization is still in progress, a `409` `Conflict` error will be
  returned.    <br><br>Please note that **this endpoint can be authorized with a
  publisher (X-Publisher-Token) or JWT (Bearer) token**. Depending on how you
  integrate with Cleeng (directly or through middleware), use either a
  <<glossary:JWT>> or X-Publisher-Token header authorization. <br> <br> <span
  style="color:green">**Please use JWT (Bearer) token to try out the endpoint in
  the API console in this documentation**.</span>
api:
  file: test.json
  operationId: register-apple-sk2-purchase
hidden: false
---