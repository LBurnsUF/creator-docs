---
title: ConfigSnapshot
type: class
superclass: Object
tags: [NotCreatable, NotReplicated]
---

# ConfigSnapshot

A snapshot of configuration values at a given version. Can be player-specific.

**Inherits from:** `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

An object with the configuration values at a specific version. A snapshot can
be targeted to a single player to apply experimentation values. This is
returned by `Class.ConfigService:GetConfigAsync()` and
`Class.ConfigService:GetConfigForPlayerAsync()`.

For more information, see
[Experience configs](../../../production/configs.md).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ConfigSnapshot.Error` | `Enum.ConfigSnapshotErrorState` | [ReadOnly] [NotReplicated] |
| `Class.ConfigSnapshot.Outdated` | `bool` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.ConfigSnapshot:GetValue`

``GetValue(key: `string`)`` -> `Variant`

### `Class.ConfigSnapshot:GetValueChangedSignal`

``GetValueChangedSignal(key: `string`)`` -> `Datatype.RBXScriptSignal`

### `Class.ConfigSnapshot:Refresh`

``Refresh()`` -> `null`

## Events

### `Class.ConfigSnapshot.UpdateAvailable`

Fires with: ()
