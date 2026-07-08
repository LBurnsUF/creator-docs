---
title: ExperienceService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ExperienceService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.ExperienceService:ExecuteCrossExperienceCall`

``ExecuteCrossExperienceCall(callId: `string`, params: `Dictionary`, successCallback: `Datatype.Function`, errorCallback: `Datatype.Function`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.ExperienceService:GetFollowUserId`

``GetFollowUserId()`` -> `int64`
   {security: RobloxScriptSecurity}

### `Class.ExperienceService:GetPendingJoinAttempt`

``GetPendingJoinAttempt()`` -> `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.ExperienceService:GetPlaceJoinState`

``GetPlaceJoinState()`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.ExperienceService:GetQueuePosition`

``GetQueuePosition()`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.ExperienceService:LaunchExperience`

``LaunchExperience(params: `Dictionary`)`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.ExperienceService:LaunchExperienceFromSource`

``LaunchExperienceFromSource(params: `Dictionary`, source: `string`)`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.ExperienceService:LaunchExperienceFromSourceWithCallback`

``LaunchExperienceFromSourceWithCallback(params: `Dictionary`, source: `string`, callback: `Datatype.Function`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.ExperienceService:RegisterForExperienceJoin`

``RegisterForExperienceJoin(callback: `Datatype.Function`)`` -> `Datatype.RBXScriptConnection`
   {security: RobloxScriptSecurity}

### `Class.ExperienceService:RegisterForExperienceLeave`

``RegisterForExperienceLeave(callback: `Datatype.Function`)`` -> `Datatype.RBXScriptConnection`
   {security: RobloxScriptSecurity}

### `Class.ExperienceService:StartCrossExperience`

``StartCrossExperience(type: `string`, params: `Dictionary`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.ExperienceService:StopCrossExperience`

``StopCrossExperience(type: `string`, params: `Dictionary`)`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.ExperienceService.OnCrossExperienceStarted`

Fires with: (type: `string`, params: `Dictionary`)

### `Class.ExperienceService.OnCrossExperienceStopped`

Fires with: (type: `string`, params: `Dictionary`)

### `Class.ExperienceService.OnNewJoinAttempt`

Fires with: (params: `Dictionary`)

### `Class.ExperienceService.PlaceJoinStateChanged`

Fires with: (state: `string`)

### `Class.ExperienceService.QueuePositionChanged`

Fires with: (position: `int`)
