---
title: InstanceFileSyncService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# InstanceFileSyncService

A service for interacting with file sync from a plugin.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

The `InstanceFileSyncService` service provides an interface for plugins to
interact with the file sync system (currently known as **Script Sync**). It
allows querying the sync status of instances and retrieving instances based on
file paths.

## Methods

### `Class.InstanceFileSyncService:GetAllInstances`

``GetAllInstances()`` -> `Datatype.Instances`
   {security: PluginSecurity}

### `Class.InstanceFileSyncService:GetStatus`

``GetStatus(instance: `Class.Instance`)`` -> `Enum.InstanceFileSyncStatus`
   {security: PluginSecurity}

### `Class.InstanceFileSyncService:GetSyncedInstance`

``GetSyncedInstance(filePath: `string`)`` -> `Class.Instance`
   {security: PluginSecurity}

### `Class.InstanceFileSyncService:GetSyncingCollaborators`

``GetSyncingCollaborators(instance: `Class.Instance`)`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.InstanceFileSyncService:GetTooltip`

``GetTooltip(instance: `Class.Instance`)`` -> `string?`
   {security: RobloxScriptSecurity}

## Events

### `Class.InstanceFileSyncService.StatusChanged`

Fires with: (instance: `Class.Instance`, status: `Enum.InstanceFileSyncStatus`)

### `Class.InstanceFileSyncService.SyncingCollaboratorsChanged`

Fires with: (instance: `Class.Instance`)
