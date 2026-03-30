---
title: Create plan
excerpt: >-
  A request to create a new plan.

  A plan is the basis for a contract with recurring payments. It is not assigned
  to a specific debtorId and can be used across multiple contracts like a
  template. After a contract is assigned to a plan with phases and options,
  usages are created which result in billable items for the debtor.

  Creating options while creating a plan is deprecated: Use the Option API
  instead to manage Options and reference them when creating a plan.
api:
  file: tst.json
  operationId: createPlan_v2
hidden: false
---