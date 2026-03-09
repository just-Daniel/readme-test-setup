---
title: Bulk User Attributes
excerpt: >
  This endpoint allows clients to submit multiple user attribute updates in
  bulk, accepting up to 256 payloads per request. Each request is validated, and
  a unique batch ID is returned for tracking the status of the batch.


  Scopes Required: [attributes:write subscriptions:write]


  Default Rate Limit: 100 requests per second
api:
  file: new-test2.json
  operationId: postBulkUserAttributes
hidden: false
---