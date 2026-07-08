---
title: CollectionService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# CollectionService

A service which manages instance collections using assigned tags.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

`CollectionService` manages groups (collections) of instances with **tags**.
Tags are sets of strings applied to instances that replicate from the server
to the client. They are also serialized when places are saved.

The primary use of `CollectionService` is to register instances with specific
tags that you can use to extend their behavior. If you find yourself adding
the same script to many different instances, a script that uses
`CollectionService` may be better.

Tags can be added or removed through this class' methods such as
`Class.CollectionService:AddTag()|AddTag()` or
`Class.CollectionService:RemoveTag()|RemoveTag()`. They can also be managed
directly in Studio through the
[Tags](../../../studio/properties.md#instance-tags) section of an instance's
properties.

##### Replication

When tags replicate, **all tags on an instance replicate at the same time**.
Therefore, if you set a tag on an instance from the client then add/remove a
**different** tag on the same instance from the server, the client's local
tags on the instance are overwritten. In
`Class.Workspace.StreamingEnabled|StreamingEnabled` places, instances can be
unloaded as they leave the client's streamed area. If such an instance
re-enters the streamed area, properties and tags will be re-synchronized from
the server. This can cause changes made by `Class.LocalScript|LocalScripts` to
be overwritten/removed.

## Methods

### `Class.CollectionService:AddTag`

``AddTag(instance: `Class.Instance`, tag: `string`)`` -> `null`
  [CustomLuaState]

### `Class.CollectionService:GetAllTags`

``GetAllTags()`` -> `Array`

### `Class.CollectionService:GetCollection`

``GetCollection(class: `string`)`` -> `Datatype.Instances`
  [Deprecated]

### `Class.CollectionService:GetInstanceAddedSignal`

``GetInstanceAddedSignal(tag: `string`)`` -> `Datatype.RBXScriptSignal`

### `Class.CollectionService:GetInstanceRemovedSignal`

``GetInstanceRemovedSignal(tag: `string`)`` -> `Datatype.RBXScriptSignal`

### `Class.CollectionService:GetTagged`

``GetTagged(tag: `string`)`` -> `Datatype.Instances`

### `Class.CollectionService:GetTags`

``GetTags(instance: `Class.Instance`)`` -> `Array`
  [CustomLuaState]

### `Class.CollectionService:HasTag`

``HasTag(instance: `Class.Instance`, tag: `string`)`` -> `bool`
  [CustomLuaState]

### `Class.CollectionService:RemoveTag`

``RemoveTag(instance: `Class.Instance`, tag: `string`)`` -> `null`
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
