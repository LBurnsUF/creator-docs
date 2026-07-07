---
title: FaceAnimatorService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# FaceAnimatorService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **AudioAnimationEnabled**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **FaceTrackingStatusEnum**: `TrackerFaceTrackingStatus` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **FlipHeadOrientation**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **VideoAnimationEnabled**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **GetTrackerLodController**() -> `TrackerLodController`
- **Init**(`videoEnabled: bool`, `audioEnabled: bool`) -> `null`
- **IsStarted**() -> `bool`
- **Start**() -> `null`
- **Step**() -> `null`
- **Stop**() -> `null`

## Events

- **TrackerError**(`error: TrackerError`)
- **TrackerPrompt**(`prompt: TrackerPromptEvent`)
