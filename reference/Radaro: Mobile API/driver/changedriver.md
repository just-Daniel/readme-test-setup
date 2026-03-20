---
title: Change driver
excerpt: >-
  The list of possible vehicle types can be found in another api.

  The skill_set_ids field allows you to set the list of skills. 

  Send "skill_set_ids": [] or "skill_set_ids": null to remove all open skills. 

  If you do not want to change the skill list, do not use this field.

  Similarly to the wayback_hub_ids.


  In case you'd like to remove skills with jobs-unassign option, use
  `?force=True` query parameter.
api:
  file: tst_fixed_v2.json
  operationId: ChangeDriver
hidden: false
---