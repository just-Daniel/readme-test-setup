---
title: Custom Attributes
excerpt: >
  Make a call to this endpoint for any attribute-based data. There are no limits
  to the amount of custom attributes that can be created. Note that you can
  create net-new properties with this API, however, it cannot be used to create
  new values for an existing UI-created property name. If a property name is
  created through the Attentive platform, all possible property values must also
  be defined in the platform. For example, if a property has possible values of
  "Adult, Teen, Children's", those are the only values that will be accepted
  through the API. This does not apply for properties with the type "Custom
  input", for example: Full Name. Also, please note that the API does not
  support arrays. For example, attempting to pass an array such as '["chicago",
  "new york"]' for an attribute like 'favorite_city' will result in a 400 error.


  **Note : The maximum length for an attribute name is 200 characters.**
api:
  file: new-test.json
  operationId: postCustomAttributes
hidden: false
---