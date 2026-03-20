---
title: Get order path
excerpt: >-
  The amount of {status: locations} pairs in `path` can vary depending on status
  change history of an order.

  Possible status values are: `pickup`, `in_progress`, `way_back`. 

  Path within `picked_up` status is not included into final result.
api:
  file: tst_fixed_v2.json
  operationId: GetOrderPath
hidden: false
---