---
title: FeatureRestrictionManager
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# FeatureRestrictionManager

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Events

- **FeatureTimeoutAttempt**(`permanent: bool`, `startTime: int64`, `duration: int64`, `featureRestrictionAbuseVector: FeatureRestrictionAbuseVector`)
- **FeatureTimeoutRestored**(`featureRestrictionAbuseVector: FeatureRestrictionAbuseVector`)
- **ShowFeatureInterventionDetails**(`featureRestrictionAbuseVector: FeatureRestrictionAbuseVector`)
- **ShowFeatureInterventionDetailsV2**(`featureRestrictionAbuseVector: FeatureRestrictionAbuseVector`, `isGameJoin: bool`)
- **TimeoutChatAttempt**(`isPermanentTimeout: bool`, `endTime: int64`)
