---
title: Object
type: class
superclass: <<<ROOT>>>
tags: [NotCreatable, NotReplicated]
---

# Object


**Tags:** [NotCreatable] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.Object.ClassName` | `string` | [ReadOnly] [NotReplicated] |
| `Class.Object.className` | `string` | [ReadOnly] [NotReplicated] [Deprecated] |

## Methods

### `Class.Object:GetPropertyChangedSignal`

``GetPropertyChangedSignal(property: `string`)`` → `Datatype.RBXScriptSignal`

### `Class.Object:IsA`

``IsA(className: `string`)`` → `bool`
  [CustomLuaState]

### `Class.Object:isA`

``isA(className: `string`)`` → `bool`
  [Deprecated] [CustomLuaState]

## Events

### `Class.Object.Changed`

Fires with: (property: `string`)
