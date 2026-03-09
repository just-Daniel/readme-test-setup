---
title: Create or update a single user with attributes, subscriptions, and identifiers
excerpt: >
  Creates or updates a single user record, including associated attributes,
  subscriptions, and identifiers. If a user with the provided identifiers
  already exists, their information will be updated; otherwise, a new user will
  be created.


  There is a limit of 100 of custom attributes that can be created. If intending
  to update an existing attribute, the name of the key must match the name of
  the existing attribute. If an existing attribute does not exist, a new
  attribute will be created with the given key as the name. Attributes with
  enumerated values must have a value that matches an existing enum value; new
  enum values will not be created.  Attempting to pass custom attributes as an
  array or a map such as `["New York City]` or `{"favorite city": "Boston"}`
  will result in a 400 error.


  Default Rate Limit: 150 requests per second
api:
  file: new-test2.json
  operationId: postUserAttributes
hidden: false
---