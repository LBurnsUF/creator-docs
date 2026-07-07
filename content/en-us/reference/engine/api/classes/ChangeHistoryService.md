---
title: ChangeHistoryService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# ChangeHistoryService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **FinishRecording**(`identifier: string`, `operation: FinishRecordingOperation`, `finalOptions: Dictionary?`) -> `null`
- **GetCanRedo**() -> `Tuple`
- **GetCanUndo**() -> `Tuple`
- **IsRecordingInProgress**(`identifier: string?`) -> `bool`
- **Redo**() -> `null`
- **ResetWaypoints**() -> `null`
- **SetEnabled**(`state: bool`) -> `null`
- **SetWaypoint**(`name: string`) -> `null`
- **TryBeginRecording**(`name: string`, `displayName: string?`) -> `string?`
- **Undo**() -> `null`

## Events

- **OnRecordingFinished**(`name: string`, `displayName: string?`, `identifier: string?`, `operation: FinishRecordingOperation`, `finalOptions: Dictionary?`)
- **OnRecordingStarted**(`name: string`, `displayName: string?`)
- **OnRedo**(`waypoint: string`)
- **OnUndo**(`waypoint: string`)
