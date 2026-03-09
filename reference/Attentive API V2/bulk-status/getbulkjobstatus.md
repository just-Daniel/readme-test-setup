---
title: Retrieve the status of a bulk ingestion job
excerpt: >
  Checks the status of a bulk ingestion job identified by bulkJobId. This
  endpoint returns the current state of the job (e.g. `PENDING`, `IN_PROGRESS`,
  `COMPLETED`, `FAILED`) along with metadata such as timestamps and error
  messages if applicable.


  If the job has completed successfully, the response includes a downloadable
  link to a `.jsonl` (JSON Lines) file containing a record of each request and
  its corresponding response. User's can audit results or process downstream
  outcomes of the bulk operation. You can fetch requests up to 2 weeks old.


  Scopes Required: No Additional scopes required.


  Default Rate Limit: 100 requests per second
api:
  file: new-test2.json
  operationId: getBulkJobStatus
hidden: false
---