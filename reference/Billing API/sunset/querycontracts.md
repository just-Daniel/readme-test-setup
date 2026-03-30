---
title: Query contracts (unpaged)
excerpt: >-
  | &#x26A0; <b>This operation has been deprecated and will be removed in the
  future!</b> &#x26A0;<br>Reason: Use the paged query endpoint instead.<br>This
  operation is replaced by <a
  href='https://docs.nitrobox.io/reference/querycontractspageable'>https://docs.nitrobox.io/reference/querycontractspageable</a>.
  |

  |
  -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  |

  | Deprecated since: 2024-09-16<br><p style='color:red;font-weight:bold'>Sunset
  at the latest:
  2025-10-01</p>                                                                                                                                                                                                         
  |

  | Please refer to our "API Lifecycle Management" and our "API Migration Guide"
  to find out
  more.                                                                                                                                                                                                                     
  |

  Returns list with 100 contracts. Contracts are sorted by default in descending
  order by contractId. This can be changed with the optional direction and
  orderBy parameters.NOTE: When searching for 'taxLocation' or
  'performanceLocation', the response will also include contracts that were set
  to the value in the past.
api:
  file: tst.json
  operationId: queryContracts
deprecated: true
hidden: false
---