---
title: DataModelPatchService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# DataModelPatchService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.DataModelPatchService:GetLuaVersion`

``GetLuaVersion(patchName: `string`)`` → `string`
   {security: RobloxScriptSecurity}

### `Class.DataModelPatchService:GetPatch`

``GetPatch(patchName: `string`)`` → `Class.Instance`
   {security: RobloxScriptSecurity}

### `Class.DataModelPatchService:RegisterPatch`

``RegisterPatch(patchName: `string`, behaviorName: `string`, localConfigPath: `string`, userId: `int64`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.DataModelPatchService:UpdatePatch`

``UpdatePatch(userId: `int64`, patchName: `string`, callbackFunction: `Datatype.Function`)`` → `null`
   {security: RobloxScriptSecurity}
