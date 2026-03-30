---
title: Query plans
excerpt: >-
  | &#x26A0; <b>This operation has been deprecated and will be removed in the
  future!</b> &#x26A0;<br>Reason: Use correct pageable query endpoint
  instead.<br>This operation is replaced by <a
  href='https://docs.nitrobox.io/reference/getallplanspageable_v2'>https://docs.nitrobox.io/reference/getallplanspageable_v2</a>.
  |

  |
  --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  |

  | Deprecated since: 2024-12-20<br><p style='color:red;font-weight:bold'>Sunset
  at the latest:
  2026-01-01</p>                                                                                                                                                                                                                
  |

  | Please refer to our "API Lifecycle Management" and our "API Migration Guide"
  to find out
  more.                                                                                                                                                                                                                            
  |

  Get a list of all plans. To reduce the result set, please use the RSQL
  query.The plan list is sorted in descending order by the planId.The sorted
  order can be changed with help of the optional direction and orderBy
  parameters.
api:
  file: tst.json
  operationId: getAllPlans_v2
deprecated: true
hidden: false
---