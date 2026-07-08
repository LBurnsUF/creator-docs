---
title: ObjectValue
type: class
superclass: ValueBase
---

# ObjectValue

A container object for a reference to another instance.

**Inherits from:** `Class.ValueBase` > `Class.Instance` > `Class.Object`

## Description

Stores a single reference to another object. If this object is duplicated
within Studio and the value refers to an object also being copied, then the
new `ObjectValue` points to the copied object instead of the original.
Otherwise, the same value is kept. Copying and pasting this object clears the
value field.

Like all `Class.ValueBase` objects, this single value is stored in the
`Class.ObjectValue.Value|Value` property. The `Changed` event fires with the
new value being stored in the object, instead of a string representing the
property being changed.

If [streaming](../../../workspace/streaming/index.md) is enabled, the `Value`
property is nil until the referenced object streams in, at which point the
`Changed` event fires.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ObjectValue.Value` | `Class.Instance` |  |

## Events

### `Class.ObjectValue.Changed`

Fires with: (value: `Class.Instance`)

### `Class.ObjectValue.changed`

Fires with: (value: `Class.Instance`)
  [Deprecated]
