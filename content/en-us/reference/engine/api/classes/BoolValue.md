---
title: BoolValue
type: class
superclass: ValueBase
---

# BoolValue

A container object for a single boolean value.

**Inherits from:** `Class.ValueBase` > `Class.Instance` > `Class.Object`

## Description

Stores a single boolean value. The value can be used for many things,
including to communicate between scripts.

Like all `Class.ValueBase` objects, this single value is stored in the
`Class.BoolValue.Value|Value` property. The `Changed` event fires with the new
value being stored in the object, instead of a string representing the
property being changed.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.BoolValue.Value` | `bool` |  |

## Events

### `Class.BoolValue.Changed`

Fires with: (value: `bool`)

### `Class.BoolValue.changed`

Fires with: (value: `bool`)
  [Deprecated]
