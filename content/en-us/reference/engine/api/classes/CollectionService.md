---
title: CollectionService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# CollectionService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **AddTag**(`instance: Instance`, `tag: string`) -> `null` [CustomLuaState]
- **GetAllTags**() -> `Array`
- **GetCollection**(`class: string`) -> `Instances` [Deprecated]
- **GetInstanceAddedSignal**(`tag: string`) -> `RBXScriptSignal`
- **GetInstanceRemovedSignal**(`tag: string`) -> `RBXScriptSignal`
- **GetTagged**(`tag: string`) -> `Instances`
- **GetTags**(`instance: Instance`) -> `Array` [CustomLuaState]
- **HasTag**(`instance: Instance`, `tag: string`) -> `bool` [CustomLuaState]
- **RemoveTag**(`instance: Instance`, `tag: string`) -> `null` [CustomLuaState]

## Events

- **ItemAdded**(`instance: Instance`) [Deprecated]
- **ItemRemoved**(`instance: Instance`) [Deprecated]
- **TagAdded**(`tag: string`)
- **TagRemoved**(`tag: string`)
