---
title: 交易单列表查询
excerpt: "* **权限异常**\n\n```\nhttp status：401\n{\n\_\_\_\_\"errorMessage\":\"invalid api key\"\n}\n```\n\n* <span class=\"colour\" style=\"color:rgb(0, 0, 0)\">**参数异常**</span>\n\n```\nhttp status：400\n{\n\"errorMessage\": \"limit must be less than or equal to 100\"\n}\n```"
api:
  file: swaggerApi.json
  operationId: get_v1-transactions
hidden: false
---