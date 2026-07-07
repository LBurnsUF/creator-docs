---
title: InstanceFileSyncService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# InstanceFileSyncService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **GetAllInstances**() -> `Instances`
- **GetStatus**(`instance: Instance`) -> `InstanceFileSyncStatus`
- **GetSyncedInstance**(`filePath: string`) -> `Instance`
- **GetSyncingCollaborators**(`instance: Instance`) -> `Array`
- **GetTooltip**(`instance: Instance`) -> `string?`

## Events

- **StatusChanged**(`instance: Instance`, `status: InstanceFileSyncStatus`)
- **SyncingCollaboratorsChanged**(`instance: Instance`)
