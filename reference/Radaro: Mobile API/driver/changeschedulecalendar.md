---
title: Change ScheduleCalendar
excerpt: >-
  You can add or overwrite the day of the temporary schedule by sending
  "2021-01-27": { "start": "4:00", "end": "11:00", "day_off": false }

  or "2021-01-27": { "day_off": true }


  You can delete the day of the temporary schedule by sending "2021-01-27": {}
  or "2021-01-28": { "day_off": false }
api:
  file: tst_fixed_v2.json
  operationId: ChangeSchedulecalendar
hidden: false
---