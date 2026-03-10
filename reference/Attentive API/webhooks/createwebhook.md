---
title: Create webhook
excerpt: |
  Make an API call to this endpoint to subscribe to a webhook.

  Events are a collection of strings of the following types:
  * `sms.subscribed`
  * `sms.sent`
  * `sms.message_link_click`
  * `email.subscribed`
  * `email.unsubscribed`
  * `email.message_link_click`
  * `email.opened`
  * `custom_attribute.set`

  Event types are case sensitive.

  All events included will be sent to the URL.
api:
  file: new-test.json
  operationId: createWebhook
hidden: false
---