---
title: DataModelPatchService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# DataModelPatchService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **GetLuaVersion**(`patchName: string`) -> `string`
- **GetPatch**(`patchName: string`) -> `Instance`
- **RegisterPatch**(`patchName: string`, `behaviorName: string`, `localConfigPath: string`, `userId: int64`) -> `null`
- **UpdatePatch**(`userId: int64`, `patchName: string`, `callbackFunction: Function`) -> `null`
