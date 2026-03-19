---
title: Delete a user
excerpt: >-
  Deletes a user by ID. By default performs a soft delete (sets deleted_at, data
  remains). Use ?force=true to permanently remove the user and cascade-delete
  all associated data (groups, auth providers, wallets, files, terms
  acceptances, etc.). This action is irreversible.
api:
  file: openapi.json
  operationId: adminDeleteUser
hidden: false
---