---
title: CollaboratorsService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# CollaboratorsService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.CollaboratorsService:GetCollaboratorsList`

``GetCollaboratorsList()`` -> `Datatype.Instances`
   {security: RobloxScriptSecurity}

### `Class.CollaboratorsService:GetSelectionHighlightsEnabled`

``GetSelectionHighlightsEnabled()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.CollaboratorsService:MultiGetCanCollaborate`

``MultiGetCanCollaborate(userIds: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CollaboratorsService:RequestFlyToCollaborator`

``RequestFlyToCollaborator(collaboratorId: `int64`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CollaboratorsService:ToggleSelectionHighlights`

``ToggleSelectionHighlights(showHighlights: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CollaboratorsService:ToggleTeamCreate`

``ToggleTeamCreate(on: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.CollaboratorsService.CollaboratorIdleUpdate`

Fires with: (collaboratorId: `int64`, isIdle: `bool`)

### `Class.CollaboratorsService.CollaboratorInstanceCreatedSignal`

Fires with: (collaboratorId: `int64`)

### `Class.CollaboratorsService.CollaboratorInstanceDestroyedSignal`

Fires with: (collaboratorId: `int64`)

### `Class.CollaboratorsService.CollaboratorStatusUpdatedSignal`

Fires with: (collaboratorId: `int64`, newStatus: `Enum.CollaboratorStatus`)

### `Class.CollaboratorsService.MultiGetCanCollaborateRetrieved`

Fires with: (requestId: `string`, canCollaborateResponses: `Array`)

### `Class.CollaboratorsService.ServerMultiGetCanCollaborateRequested`

Fires with: (userIds: `string`)

### `Class.CollaboratorsService.ToggleSelectionHighlightsSignal`

Fires with: (areHighlightsShown: `bool`)
