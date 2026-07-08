---
title: IntConstrainedValue
type: class
superclass: ValueBase
tags: [Deprecated]
---

# IntConstrainedValue

An IntConstrainedValue is used to store a value which can never be less than
MinValue and can never be more than MaxValue.

**Inherits from:** `Class.ValueBase` > `Class.Instance` > `Class.Object`

**Tags:** [Deprecated]

## Description

An IntConstrainedValue is used to store a value which can never be less than
MinValue and can never be more than MaxValue.

> **Deprecated:** The IntConstrainedValue object has been deprecated as developers can now use
the `Library.math.clamp()` function to constrain values.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.IntConstrainedValue.ConstrainedValue` | `int64` | [Hidden] [NotReplicated] |
| `Class.IntConstrainedValue.MaxValue` | `int64` |  |
| `Class.IntConstrainedValue.MinValue` | `int64` |  |
| `Class.IntConstrainedValue.Value` | `int64` | [NotReplicated] |

## Events

### `Class.IntConstrainedValue.Changed`

Fires with: (value: `int64`)

### `Class.IntConstrainedValue.changed`

Fires with: (value: `int64`)
  [Deprecated]
