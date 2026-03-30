---
title: Reissue document
excerpt: >-
  Reissue a specific document to have that document updated with corrected data.
  Within a Reissue, a document can be corrected because of the wrong invoice- or
  shipping address. Generally, a reissue leads always to a credit note that
  includes the reversed data from the corrected document and a new invoice with
  corrected data as the correction invoice. You can perform a reissue with new
  data in the request or update the customer data beforehand, but you cannot
  reissue the same document twice. Furthermore, the new address data sent in the
  request will not only update the address for the correction invoice but also
  update the address in the customer data. In case of shipping address
  correction, if the reissue address does not have a shipping address, a new
  shipping address will be created for the customer. The reissue can be also
  used to perform some template changes that are made beforehand and should be
  reflected on the correction invoice.
api:
  file: tst.json
  operationId: reissuedocument
hidden: false
---