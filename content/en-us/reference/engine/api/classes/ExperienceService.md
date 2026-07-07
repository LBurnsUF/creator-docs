---
title: ExperienceService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ExperienceService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **ExecuteCrossExperienceCall**(`callId: string`, `params: Dictionary`, `successCallback: Function`, `errorCallback: Function`) -> `null`
- **GetFollowUserId**() -> `int64`
- **GetPendingJoinAttempt**() -> `Dictionary`
- **GetPlaceJoinState**() -> `string`
- **GetQueuePosition**() -> `int`
- **LaunchExperience**(`params: Dictionary`) -> `string`
- **LaunchExperienceFromSource**(`params: Dictionary`, `source: string`) -> `string`
- **LaunchExperienceFromSourceWithCallback**(`params: Dictionary`, `source: string`, `callback: Function`) -> `null`
- **RegisterForExperienceJoin**(`callback: Function`) -> `RBXScriptConnection`
- **RegisterForExperienceLeave**(`callback: Function`) -> `RBXScriptConnection`
- **StartCrossExperience**(`type: string`, `params: Dictionary`) -> `null`
- **StopCrossExperience**(`type: string`, `params: Dictionary`) -> `null`

## Events

- **OnCrossExperienceStarted**(`type: string`, `params: Dictionary`)
- **OnCrossExperienceStopped**(`type: string`, `params: Dictionary`)
- **OnNewJoinAttempt**(`params: Dictionary`)
- **PlaceJoinStateChanged**(`state: string`)
- **QueuePositionChanged**(`position: int`)
