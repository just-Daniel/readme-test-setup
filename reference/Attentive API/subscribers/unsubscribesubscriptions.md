---
title: Unsubscribe subscriptions for a user
excerpt: >
  Make a call to this endpoint to unsubscribe a user from a subscription type or
  channel. If no subscriptions

  are present in the request, the user is unsubscribed from all subscriptions.
  If subscriptions are present

  in the request, the user is unsubscribed from the requested type or channel
  combination. By default, if a

  subscription exists, but the user is already unsubscribed, it records the
  attempt to unsubscribe the

  subscription again. For TEXT subscriptions, a message is sent to the person
  indicating that they are

  unsubscribed.


  For the user object, the email data point determines which email subscriptions
  a user has and the phone data point 

  determines which text (or sms) subscriptions a user has. Passing in an email
  does not locate, nor unsubscribe, 

  a user from any sms subscriptions. Similarly, passing in a phone does not
  locate, nor unsubscribe, a user from any email subscriptions.
api:
  file: new-test.json
  operationId: unsubscribeSubscriptions
hidden: false
---