---
title: List users
excerpt: >-
  Lists users with optional filters. Admins can list all users across tenants or
  filter by tenant_id. Non-admins are auto-filtered to their own tenant.
  Searchable by group_id (exact match), username (partial), first_name
  (partial), last_name (partial), or user_id (exact match). Admins can include
  soft-deleted users with include_deleted=true.
api:
  file: openapi.json
  operationId: listUsers
hidden: false
---