---
title: CollaboratorsService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# CollaboratorsService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **GetCollaboratorsList**() -> `Instances`
- **GetSelectionHighlightsEnabled**() -> `bool`
- **MultiGetCanCollaborate**(`userIds: string`) -> `null`
- **RequestFlyToCollaborator**(`collaboratorId: int64`) -> `null`
- **ToggleSelectionHighlights**(`showHighlights: bool`) -> `null`
- **ToggleTeamCreate**(`on: bool`) -> `null`

## Events

- **CollaboratorIdleUpdate**(`collaboratorId: int64`, `isIdle: bool`)
- **CollaboratorInstanceCreatedSignal**(`collaboratorId: int64`)
- **CollaboratorInstanceDestroyedSignal**(`collaboratorId: int64`)
- **CollaboratorStatusUpdatedSignal**(`collaboratorId: int64`, `newStatus: CollaboratorStatus`)
- **MultiGetCanCollaborateRetrieved**(`requestId: string`, `canCollaborateResponses: Array`)
- **ServerMultiGetCanCollaborateRequested**(`userIds: string`)
- **ToggleSelectionHighlightsSignal**(`areHighlightsShown: bool`)
