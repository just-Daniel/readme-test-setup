---
title: Update option
excerpt: >-
  Updates a option. If it's in DRAFT status (it's not assigned to any plans yet)
  the changes will be made immediately. 

  If it's in FINAL status, RatedUsageOptions cannot be updated anymore. 

  For other types of Options the new option version will be used in the billing
  periods following the valid_from.
api:
  file: tst.json
  operationId: updateOption_v2
hidden: false
---