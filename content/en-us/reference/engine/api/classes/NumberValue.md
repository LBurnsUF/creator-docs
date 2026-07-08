---
title: NumberValue
type: class
superclass: ValueBase
---

# NumberValue

A container object for a single double-precision floating point number.

**Inherits from:** `Class.ValueBase` > `Class.Instance` > `Class.Object`

## Description

Store a single [Luau number](https://luau.org/syntax#number-literals), defined
to be
[double-precision floating point number](https://en.wikipedia.org/wiki/Double-precision_floating-point_format),
or more commonly known as a **double**. This stores a number in 64 bits (8
bytes) using the IEEE 754 representation (1 sign bit, 11 exponent bits and 52
fractional bits). Maximum and minimum values are
&PlusMinus;1.7976931348623157e+308, with a range of &PlusMinus;2^53 for exact
integer representations.

Like all `Class.ValueBase` objects, this single value is stored in the
`Class.NumberValue.Value|Value` property. The `Changed` event fires with the
new value being stored in the object, instead of a string representing the
property being changed.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.NumberValue.Value` | `double` |  |

## Events

### `Class.NumberValue.Changed`

Fires with: (value: `double`)

### `Class.NumberValue.changed`

Fires with: (value: `double`)
  [Deprecated]
