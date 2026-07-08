---
title: StringValue
type: class
superclass: ValueBase
---

# StringValue

A container object for a single string.

**Inherits from:** `Class.ValueBase` > `Class.Instance` > `Class.Object`

## Description

Stores a single [Luau string](https://luau.org/syntax#string-literals). The
length of the string can't be more than 200,000 characters; anything longer
causes a `String too long` error.

If the string is too long to be displayed in the **Value** field within the
**Properties** window, it shows partial string contents and an ellipsis (...).

Like all `Class.ValueBase` objects, this single value is stored in the
`Class.StringValue.Value|Value` property. The `Changed` event fires with the
new value being stored in the object, instead of a string representing the
property being changed.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.StringValue.Value` | `string` |  |

## Events

### `Class.StringValue.Changed`

Fires with: (value: `string`)

### `Class.StringValue.changed`

Fires with: (value: `string`)
  [Deprecated]
