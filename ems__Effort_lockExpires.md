---
exo__Asset_isDefinedBy: "[[f6e01f7a-d727-494a-82a3-815597d33e86]]"
exo__Asset_uid: e9f50a85-ccd2-4781-9b09-2a45e5e40b99
exo__Asset_createdAt: 2026-04-27T23:59:15
exo__Asset_updatedAt: 2026-04-27T23:59:15
exo__Asset_createdBy: "[[de20a3f1-7483-4714-ab28-b45f5cf02c76|ExoAssistant]]"
exo__Instance_class:
  - "[[exo__TimestampProperty]]"
  - "[[exo__NonInheritableProperty]]"
exo__Property_domain: "[[ems__Effort]]"
exo__Asset_label: "ems__Effort_lockExpires"
exo__Asset_relates:
  - "[[ad46456a-fa1a-487c-b51e-ac3a8706bba1|RFC ems-locks v1]]"
---

Lock TTL boundary (ISO 8601 with timezone). Default acquire-time = NOW + 2h (heartbeat baseline per RFC 1f1eb6a4). Cardinality 0..1, paired с `ems__Effort_lockedBy`.

CQ2 — expired locks (zombie cleanup): `FILTER(STR(?expires) <= "<NOW-ISO8601>")`.
