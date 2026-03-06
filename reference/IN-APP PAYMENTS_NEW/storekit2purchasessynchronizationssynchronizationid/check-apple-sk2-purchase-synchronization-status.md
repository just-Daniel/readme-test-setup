---
title: Check Apple SK2 purchase synchronization status
excerpt: >-
  Use this endpoint to retrieve the status and result of a purchase
  synchronization or transfer process initiated by the
  [/purchases](https://developers.cleeng.com/reference/register-apple-storekit-2-purchase)
  or
  [/purchases/transfers](https://developers.cleeng.com/reference/transfer-apple-sk2-purchase)
  endpoint. This endpoint provides a concise response with the essential status
  information, including `status`, `accessGranted`, `offerId`, and `result`.
  <br><br> The status field indicates the current stage of the synchronization
  process: <br> - `processing`: The synchronization is in progress.  <br> -
  `retrying:` The synchronization encountered an error and is being retried.
  This status may appear multiple times. <br> - `finalized:` The synchronization
  process has completed. <br><br> The `result` field provides more detailed
  information about the outcome of the synchronization and is only available
  when `status` is `finalized`. The `accessGranted` field indicates whether the
  user is entitled to the offer. The `offerId` field provides the ID of the
  offer. You can see some possible scenarios and the corresponding response
  fields in the
  [polling](https://developers.cleeng.com/docs/apple-in-app-purchase-storekit-2#polling)
  section of the integration tutorial. <br><br>Please note that **this endpoint
  can be authorized with a publisher (X-Publisher-Token) or JWT (Bearer)
  token**. Depending on how you integrate with Cleeng (directly or through
  middleware), use either a <<glossary:JWT>> or X-Publisher-Token header
  authorization. <br> <br> <span style="color:green">**Please use JWT (Bearer)
  token to try out the endpoint in the API console in this
  documentation**.</span>
api:
  file: test.json
  operationId: check-apple-sk2-purchase-synchronization-status
hidden: false
---