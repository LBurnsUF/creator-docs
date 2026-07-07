---
title: CollectionService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# CollectionService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.CollectionService:AddTag`

``AddTag(instance: `Class.Instance`, tag: `string`)`` → `null`
  [CustomLuaState]

### `Class.CollectionService:GetAllTags`

``GetAllTags()`` → `Array`

### `Class.CollectionService:GetCollection`

``GetCollection(class: `string`)`` → `Datatype.Instances`
  [Deprecated]

### `Class.CollectionService:GetInstanceAddedSignal`

``GetInstanceAddedSignal(tag: `string`)`` → `Datatype.RBXScriptSignal`

### `Class.CollectionService:GetInstanceRemovedSignal`

``GetInstanceRemovedSignal(tag: `string`)`` → `Datatype.RBXScriptSignal`

### `Class.CollectionService:GetTagged`

``GetTagged(tag: `string`)`` → `Datatype.Instances`

### `Class.CollectionService:GetTags`

``GetTags(instance: `Class.Instance`)`` → `Array`
  [CustomLuaState]

### `Class.CollectionService:HasTag`

``HasTag(instance: `Class.Instance`, tag: `string`)`` → `bool`
  [CustomLuaState]

### `Class.CollectionService:RemoveTag`

``RemoveTag(instance: `Class.Instance`, tag: `string`)`` → `null`
  [CustomLuaState]

## Events

### `Class.CollectionService.ItemAdded`

Fires with: (instance: `Class.Instance`)
  [Deprecated]

### `Class.CollectionService.ItemRemoved`

Fires with: (instance: `Class.Instance`)
  [Deprecated]

### `Class.CollectionService.TagAdded`

Fires with: (tag: `string`)

### `Class.CollectionService.TagRemoved`

Fires with: (tag: `string`)
