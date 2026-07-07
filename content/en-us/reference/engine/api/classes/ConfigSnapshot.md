---
title: ConfigSnapshot
type: class
superclass: Object
tags: [NotCreatable, NotReplicated]
---

# ConfigSnapshot

**Inherits from:** `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.ConfigSnapshot.Error` | `Enum.ConfigSnapshotErrorState` | [ReadOnly] [NotReplicated] |
| `Class.ConfigSnapshot.Outdated` | `bool` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.ConfigSnapshot:GetValue`

``GetValue(key: `string`)`` → `Variant`

### `Class.ConfigSnapshot:GetValueChangedSignal`

``GetValueChangedSignal(key: `string`)`` → `Datatype.RBXScriptSignal`

### `Class.ConfigSnapshot:Refresh`

``Refresh()`` → `null`

## Events

### `Class.ConfigSnapshot.UpdateAvailable`

Fires with: ()
