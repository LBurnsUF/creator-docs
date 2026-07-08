---
title: ChangeHistoryService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# ChangeHistoryService

**Must** be used by plugins to communicate to Studio how to undo and redo the
changes which they make to the experience.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

Plugin developers **must** use `Class.ChangeHistoryService` to tell Studio how
to undo and redo changes that their plugins make to experiences by recording.
Before making changes, a plugin calls
`Class.ChangeHistoryService:TryBeginRecording()`, remembering the identifier
it assigns, then after making changes, the Plugin calls
`Class.ChangeHistoryService:FinishRecording()` to complete the recording.

Plugins may also programmatically invoke an undo or redo through
`Class.ChangeHistoryService:Undo()` or `Class.ChangeHistoryService:Redo()`.

`Class.ChangeHistoryService` is not enabled at runtime, so calling its methods
in a running experience has no effect.

## Methods

### `Class.ChangeHistoryService:FinishRecording`

``FinishRecording(identifier: `string`, operation: `Enum.FinishRecordingOperation`, finalOptions: `Dictionary?`)`` -> `null`
   {security: PluginSecurity}

### `Class.ChangeHistoryService:GetCanRedo`

``GetCanRedo()`` -> `Tuple`
   {security: PluginSecurity}

### `Class.ChangeHistoryService:GetCanUndo`

``GetCanUndo()`` -> `Tuple`
   {security: PluginSecurity}

### `Class.ChangeHistoryService:IsRecordingInProgress`

``IsRecordingInProgress(identifier: `string?`)`` -> `bool`
   {security: PluginSecurity}

### `Class.ChangeHistoryService:Redo`

``Redo()`` -> `null`
   {security: PluginSecurity}

### `Class.ChangeHistoryService:ResetWaypoints`

``ResetWaypoints()`` -> `null`
   {security: PluginSecurity}

### `Class.ChangeHistoryService:SetEnabled`

``SetEnabled(state: `bool`)`` -> `null`
   {security: PluginSecurity}

### `Class.ChangeHistoryService:SetWaypoint`

``SetWaypoint(name: `string`)`` -> `null`
   {security: PluginSecurity}

### `Class.ChangeHistoryService:TryBeginRecording`

``TryBeginRecording(name: `string`, displayName: `string?`)`` -> `string?`
   {security: PluginSecurity}

### `Class.ChangeHistoryService:Undo`

``Undo()`` -> `null`
   {security: PluginSecurity}

## Events

### `Class.ChangeHistoryService.OnRecordingFinished`

Fires with: (name: `string`, displayName: `string?`, identifier: `string?`, operation: `Enum.FinishRecordingOperation`, finalOptions: `Dictionary?`)

### `Class.ChangeHistoryService.OnRecordingStarted`

Fires with: (name: `string`, displayName: `string?`)

### `Class.ChangeHistoryService.OnRedo`

Fires with: (waypoint: `string`)

### `Class.ChangeHistoryService.OnUndo`

Fires with: (waypoint: `string`)
