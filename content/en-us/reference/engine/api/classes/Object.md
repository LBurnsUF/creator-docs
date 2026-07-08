---
title: Object
type: class
superclass: <<<ROOT>>>
tags: [NotCreatable, NotReplicated]
---

# Object

`Object` is the base class for all classes in the Roblox class hierarchy.


**Tags:** [NotCreatable] [NotReplicated]

## Description

`Object` is the base class for all classes in the Roblox class hierarchy.
Every other class that the Roblox Engine defines inherits all of the members
of `Object`. It is not possible to directly create an `Object`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Object.ClassName` | `string` | [ReadOnly] [NotReplicated] |
| `Class.Object.className` | `string` | [ReadOnly] [NotReplicated] [Deprecated] |

## Methods

### `Class.Object:GetPropertyChangedSignal`

``GetPropertyChangedSignal(property: `string`)`` -> `Datatype.RBXScriptSignal`

### `Class.Object:IsA`

``IsA(className: `string`)`` -> `bool`
  [CustomLuaState]

### `Class.Object:isA`

``isA(className: `string`)`` -> `bool`
  [Deprecated] [CustomLuaState]

## Events

### `Class.Object.Changed`

Fires with: (property: `string`)
