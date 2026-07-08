---
title: FaceAnimatorService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# FaceAnimatorService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.FaceAnimatorService.AudioAnimationEnabled` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.FaceAnimatorService.FaceTrackingStatusEnum` | `Enum.TrackerFaceTrackingStatus` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.FaceAnimatorService.FlipHeadOrientation` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.FaceAnimatorService.VideoAnimationEnabled` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |

## Methods

### `Class.FaceAnimatorService:GetTrackerLodController`

``GetTrackerLodController()`` -> `Class.TrackerLodController`
   {security: RobloxScriptSecurity}

### `Class.FaceAnimatorService:Init`

``Init(videoEnabled: `bool`, audioEnabled: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.FaceAnimatorService:IsStarted`

``IsStarted()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.FaceAnimatorService:Start`

``Start()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.FaceAnimatorService:Step`

``Step()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.FaceAnimatorService:Stop`

``Stop()`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.FaceAnimatorService.TrackerError`

Fires with: (error: `Enum.TrackerError`)

### `Class.FaceAnimatorService.TrackerPrompt`

Fires with: (prompt: `Enum.TrackerPromptEvent`)
