---
title: FeatureRestrictionManager
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# FeatureRestrictionManager

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Events

### `Class.FeatureRestrictionManager.FeatureTimeoutAttempt`

Fires with: (permanent: `bool`, startTime: `int64`, duration: `int64`, featureRestrictionAbuseVector: `Enum.FeatureRestrictionAbuseVector`)

### `Class.FeatureRestrictionManager.FeatureTimeoutRestored`

Fires with: (featureRestrictionAbuseVector: `Enum.FeatureRestrictionAbuseVector`)

### `Class.FeatureRestrictionManager.ShowFeatureInterventionDetails`

Fires with: (featureRestrictionAbuseVector: `Enum.FeatureRestrictionAbuseVector`)

### `Class.FeatureRestrictionManager.ShowFeatureInterventionDetailsV2`

Fires with: (featureRestrictionAbuseVector: `Enum.FeatureRestrictionAbuseVector`, isGameJoin: `bool`)

### `Class.FeatureRestrictionManager.TimeoutChatAttempt`

Fires with: (isPermanentTimeout: `bool`, endTime: `int64`)
