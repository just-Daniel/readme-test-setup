---
title: Check Vizio purchase status [Beta]
excerpt: >-
  Use this endpoint to check the status of a Vizio in-app purchase. <br> The
  status returned in response can have three values: <br> <br> - `pending` -
  purchase is still being processed <br> - `success` - purchase processing has
  finished with a positive result <br> - `failure` - purchase processing has
  finished with a negative result, an error occurred during processing.<br> 
  <br>Please note that <<glossary:JWT>> (Bearer) token authorization** should be
  used** for this endpoint.
api:
  file: test.json
  operationId: check-vizio-purchase-status
hidden: false
---