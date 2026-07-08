---
title: DraftsService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# DraftsService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.DraftsService:CommitEdits`

``CommitEdits(scripts: `Datatype.Instances`)`` -> `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.DraftsService:DiscardEdits`

``DiscardEdits(scripts: `Datatype.Instances`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.DraftsService:GetDraftStatus`

``GetDraftStatus(script: `Class.Instance`)`` -> `Enum.DraftStatusCode`
   {security: RobloxScriptSecurity}

### `Class.DraftsService:GetDrafts`

``GetDrafts()`` -> `Datatype.Instances`
  [Yields] {security: RobloxScriptSecurity}

### `Class.DraftsService:GetEditors`

``GetEditors(script: `Class.Instance`)`` -> `Datatype.Instances`
   {security: RobloxScriptSecurity}

### `Class.DraftsService:RestoreScripts`

``RestoreScripts(scripts: `Datatype.Instances`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.DraftsService:ShowDiffsAgainstBase`

``ShowDiffsAgainstBase(scripts: `Datatype.Instances`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.DraftsService:ShowDiffsAgainstServer`

``ShowDiffsAgainstServer(scripts: `Datatype.Instances`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.DraftsService:ShowSourceDiffsAgainstCurrent`

``ShowSourceDiffsAgainstCurrent(sources: `Array`, scripts: `Datatype.Instances`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.DraftsService:UpdateToLatestVersion`

``UpdateToLatestVersion(scripts: `Datatype.Instances`)`` -> `null`
  [Yields] {security: RobloxScriptSecurity}

## Events

### `Class.DraftsService.CommitStatusChanged`

Fires with: (script: `Class.Instance`, status: `Enum.DraftStatusCode`)

### `Class.DraftsService.DraftAdded`

Fires with: (script: `Class.Instance`)

### `Class.DraftsService.DraftRemoved`

Fires with: (script: `Class.Instance`)

### `Class.DraftsService.DraftStatusChanged`

Fires with: (script: `Class.Instance`)

### `Class.DraftsService.EditorsListChanged`

Fires with: (script: `Class.Instance`)

### `Class.DraftsService.UpdateStatusChanged`

Fires with: (script: `Class.Instance`, status: `Enum.DraftStatusCode`)
