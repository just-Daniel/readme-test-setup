---
title: Send confirmation
excerpt: >-
  **Important!**

  This api sends data in form-data format. Json and base64 are not used here.


  Pre confirmation and confirmation data can be sent in statuses starting from
  in_progress.

  Pick up confirmation data can be sent in statuses starting from pick_up.

  Images are sent via Content-Type:multipart/form-data to fields
  pre_confirmation_signature, pre_confirmation_photos, confirmation_signature,
  confirmation_photos,

  pick_up_confirmation_signature, pick_up_confirmation_photos.

  Fields pre_confirmation_photos, confirmation_photos,
  pick_up_confirmation_photos can be used several times.
api:
  file: tst_fixed_v2.json
  operationId: SendConfirmation
hidden: false
---