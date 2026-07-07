---
title: DraftsService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# DraftsService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **CommitEdits**(`scripts: Instances`) -> `null` [Yields]
- **DiscardEdits**(`scripts: Instances`) -> `null`
- **GetDraftStatus**(`script: Instance`) -> `DraftStatusCode`
- **GetDrafts**() -> `Instances` [Yields]
- **GetEditors**(`script: Instance`) -> `Instances`
- **RestoreScripts**(`scripts: Instances`) -> `null`
- **ShowDiffsAgainstBase**(`scripts: Instances`) -> `null`
- **ShowDiffsAgainstServer**(`scripts: Instances`) -> `null`
- **ShowSourceDiffsAgainstCurrent**(`sources: Array`, `scripts: Instances`) -> `null`
- **UpdateToLatestVersion**(`scripts: Instances`) -> `null` [Yields]

## Events

- **CommitStatusChanged**(`script: Instance`, `status: DraftStatusCode`)
- **DraftAdded**(`script: Instance`)
- **DraftRemoved**(`script: Instance`)
- **DraftStatusChanged**(`script: Instance`)
- **EditorsListChanged**(`script: Instance`)
- **UpdateStatusChanged**(`script: Instance`, `status: DraftStatusCode`)
