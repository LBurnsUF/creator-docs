---
title: ExperienceStateRecordingService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# ExperienceStateRecordingService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **ExitPlayback**() -> `null`
- **GetCurrentPlaybackRestartFrames**() -> `Array`
- **GetPlaybackCurrentFrame**() -> `int64`
- **GetPlaybackMode**() -> `ExperienceStateRecordingPlaybackMode`
- **LoadPlaybackAsync**(`uri: string`, `placeFileUri: string?`, `mode: ExperienceStateRecordingLoadMode`, `sourceType: ExperienceStateRecordingLoadSourceType`) -> `Dictionary` [Yields]
- **SetPlaybackFrame**(`frame: int64`) -> `null`
- **SetPlaybackMode**(`mode: ExperienceStateRecordingPlaybackMode`) -> `null`
- **SetPlaybackPercentage**(`percentage: float`) -> `null`

## Events

- **PlaybackStatusUpdated**(`percentage: float`, `currentFrameNumber: int64`)
