---
title: ExperienceStateRecordingService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# ExperienceStateRecordingService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.ExperienceStateRecordingService:ExitPlayback`

``ExitPlayback()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.ExperienceStateRecordingService:GetCurrentPlaybackRestartFrames`

``GetCurrentPlaybackRestartFrames()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.ExperienceStateRecordingService:GetPlaybackCurrentFrame`

``GetPlaybackCurrentFrame()`` -> `int64`
   {security: RobloxScriptSecurity}

### `Class.ExperienceStateRecordingService:GetPlaybackMode`

``GetPlaybackMode()`` -> `Enum.ExperienceStateRecordingPlaybackMode`
   {security: RobloxScriptSecurity}

### `Class.ExperienceStateRecordingService:LoadPlaybackAsync`

``LoadPlaybackAsync(uri: `string`, placeFileUri: `string?`, mode: `Enum.ExperienceStateRecordingLoadMode`, sourceType: `Enum.ExperienceStateRecordingLoadSourceType`)`` -> `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.ExperienceStateRecordingService:SetPlaybackFrame`

``SetPlaybackFrame(frame: `int64`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.ExperienceStateRecordingService:SetPlaybackMode`

``SetPlaybackMode(mode: `Enum.ExperienceStateRecordingPlaybackMode`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.ExperienceStateRecordingService:SetPlaybackPercentage`

``SetPlaybackPercentage(percentage: `float`)`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.ExperienceStateRecordingService.PlaybackStatusUpdated`

Fires with: (percentage: `float`, currentFrameNumber: `int64`)
