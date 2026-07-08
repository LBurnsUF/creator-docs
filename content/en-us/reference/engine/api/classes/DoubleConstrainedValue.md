---
title: DoubleConstrainedValue
type: class
superclass: ValueBase
tags: [Deprecated]
---

# DoubleConstrainedValue

An instance which is used to create a number value which can never be less
than the MinValue or more than the MaxValue.

**Inherits from:** `Class.ValueBase` > `Class.Instance` > `Class.Object`

**Tags:** [Deprecated]

## Description

An instance which is used to create a number value which can never be less
than the MinValue or more than the MaxValue.

> **Deprecated:** The DoubleConstrainedValue object has been deprecated as developers can now
use the `Library.math.clamp()` function to constrain values.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.DoubleConstrainedValue.ConstrainedValue` | `double` | [Hidden] [NotReplicated] |
| `Class.DoubleConstrainedValue.MaxValue` | `double` |  |
| `Class.DoubleConstrainedValue.MinValue` | `double` |  |
| `Class.DoubleConstrainedValue.Value` | `double` | [NotReplicated] |

## Events

### `Class.DoubleConstrainedValue.Changed`

Fires with: (value: `double`)

### `Class.DoubleConstrainedValue.changed`

Fires with: (value: `double`)
  [Deprecated]
