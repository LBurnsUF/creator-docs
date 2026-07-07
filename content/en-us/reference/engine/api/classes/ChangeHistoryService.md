---
title: ChangeHistoryService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# ChangeHistoryService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.ChangeHistoryService:FinishRecording`

``FinishRecording(identifier: `string`, operation: `Enum.FinishRecordingOperation`, finalOptions: `Dictionary?`)`` → `null`
   {security: PluginSecurity}

### `Class.ChangeHistoryService:GetCanRedo`

``GetCanRedo()`` → `Tuple`
   {security: PluginSecurity}

### `Class.ChangeHistoryService:GetCanUndo`

``GetCanUndo()`` → `Tuple`
   {security: PluginSecurity}

### `Class.ChangeHistoryService:IsRecordingInProgress`

``IsRecordingInProgress(identifier: `string?`)`` → `bool`
   {security: PluginSecurity}

### `Class.ChangeHistoryService:Redo`

``Redo()`` → `null`
   {security: PluginSecurity}

### `Class.ChangeHistoryService:ResetWaypoints`

``ResetWaypoints()`` → `null`
   {security: PluginSecurity}

### `Class.ChangeHistoryService:SetEnabled`

``SetEnabled(state: `bool`)`` → `null`
   {security: PluginSecurity}

### `Class.ChangeHistoryService:SetWaypoint`

``SetWaypoint(name: `string`)`` → `null`
   {security: PluginSecurity}

### `Class.ChangeHistoryService:TryBeginRecording`

``TryBeginRecording(name: `string`, displayName: `string?`)`` → `string?`
   {security: PluginSecurity}

### `Class.ChangeHistoryService:Undo`

``Undo()`` → `null`
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
