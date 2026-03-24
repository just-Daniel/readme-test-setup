---
title: /v1beta/projects/{project}/findings:search
excerpt: |-
  SearchFindings is a more powerful version of ListFindings that
  supports complex queries like "findings for issues" using functions such as
  `has_issue` and `has_asset` in the query string.
  Example to search for findings for a specific issue:
  `has_issue("name=\"vaults/vault-12345/issues/issue-12345\"")`)
api:
  file: openapi.json
  operationId: SearchFindings
hidden: false
---