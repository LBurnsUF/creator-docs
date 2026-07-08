---
title: IntValue
type: class
superclass: ValueBase
---

# IntValue

A container object for a single integer.

**Inherits from:** `Class.ValueBase` > `Class.Instance` > `Class.Object`

## Description

Stores a single signed [64-bit integer](../../../luau/numbers.md#int64). The
highest allowed value is 2^63-1 or around 9.2 quintillion (9.2^18). Attempting
to store larger numbers causes an
[integer overflow](https://en.wikipedia.org/wiki/Integer_overflow). The lowest
allowed value is -2^63. Practically, however, working with integers larger
than 2^53 (9^15) causes loss of precision since Luau uses double-precision
floating-point to store numbers.

It's possible to store values between 2^53 and 2^63-1 using the
[Properties](../../../studio/properties.md) window since it uses strings to
pass data to the engine, but manipulating large values via Luau scripts
results in loss of precision and rounding as mentioned above.

The main advantage of using **IntValue** lies in its rounding of values to the
nearest integer, with halfway cases rounded away from 0. For values outside of
this range, use `Class.NumberValue` instead.

Like all `Class.ValueBase` objects, this single value is stored in the
`Class.IntValue.Value|Value` property. The `Changed` event fires with the new
value being stored in the object, instead of a string representing the
property being changed.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.IntValue.Value` | `int64` |  |

## Events

### `Class.IntValue.Changed`

Fires with: (value: `int64`)

### `Class.IntValue.changed`

Fires with: (value: `int64`)
  [Deprecated]
