---
title: View Recent Catalog Uploads
excerpt: >
  Make a call to this endpoint to list recent catalog uploads with their
  statuses to gain visibility into the ingestion workflow in order of creation.
  See the POST of this endpoint for details.

  `Expires` indicates how long you can wait before uploading the product catalog
  file. If the catalog upload expires, then we will no longer process the file
  that you upload and you will need to initiate  a new catalog upload.
api:
  file: new-test.json
  operationId: getUploads
hidden: false
---