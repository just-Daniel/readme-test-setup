---
title: Subscribe user
excerpt: >
  Make a call to this endpoint to opt-in a user to a subscription. 


  Notes:

  - A legal disclosure is required when a user is opted-in programmatically.
      - For marketing messages, required [legal language](https://docs.attentivemobile.com/pages/legal-docs/legal-disclosure-language/) must be included.

      - For transactional messages, you must include a [transactional opt-in unit](https://docs.attentivemobile.com/pages/legal-docs/legal-transactional/).
    
  - By default, if a subscription already exists, it will try and record the
  attempt to create the subscription again. For TEXT subscriptions, this will
  result in a message being sent to the person indicating that they are already
  subscribed.

  - Requests to opt-in subscribers must either contain a) a sign-up source id or
  b) both a locale and a subscription type.
      - The unique identifier of a sign-up source can be found in the Sign-up Units tab of the Attentive platform in the ID column. 
      If this value is provided in the request, then this sign-up unit will be used for opting in the user in the request.

      - Callers of this endpoint have the option to omit `signUpSourceId` and, instead, provide both a `locale` and a `subscriptionType` (see below for field details). 
      Given the locale and subscription type, Attentive will resolve any matching API opt-in units. To opt-in a user to a subscription without a `signUpSourceId` and exclusively based on locale and subscription type,
      there must be exactly one API sign-up unit that matches the provided locale and subscription type. Conversely, requests that contain a locale and a subscription type
      that do not have a corresponding sign-up unit or that have multiple matching sign-up units will receive a `400` response and will not opt a user into a subscription.

  - Phone numbers must be submitted in [e164
  format](https://en.wikipedia.org/wiki/E.164).
      - valid examples: `+19148440001`, `+442071838750`, `+551155256325`
      - invalid examples: `19148440001`, `+1---914---844---0001`, `1 () 914 844 0001`
api:
  file: new-test.json
  operationId: addSubscriptions
hidden: false
---