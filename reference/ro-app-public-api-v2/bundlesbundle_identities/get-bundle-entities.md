---
title: Get Bundle Entities
excerpt: >-
  Returns a list of entities within a particular bundle. If price of the entity
  is default, it won't be returned in the response. If a different price is
  chosen, in case it's of one of the existing price types, "price_id" field will
  be returned with a unique identifier, and in case it was manually adjusted
  "custom_price" field will be returned.
api:
  file: ro-app-public-api-v2.json
  operationId: get-bundle-entities
hidden: false
---