---
title: Axes
type: datatype
---

# `Datatype.Axes`

The `Axes` data type is for the `Class.ArcHandles` class to control which
rotation axes are currently enabled.

## Description

The `Axes` data type is for the `Class.ArcHandles` class to control which
rotation axes are currently enabled.

## Constructors

### `Axes.new`

Creates a new Axes using list of axes and/or faces. NormalIds (faces) are
converted to the corresponding axes.

**Parameters:**

- `axes`: `Tuple`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Axes.X` | `bool` | Whether the X axis is enabled. |
| `Axes.Y` | `bool` | Whether the Y axis is enabled. |
| `Axes.Z` | `bool` | Whether the Z axis is enabled. |
| `Axes.Top` | `bool` | Whether the top face is included. |
| `Axes.Bottom` | `bool` | Whether the bottom face is included. |
| `Axes.Left` | `bool` | Whether the left face is included. |
| `Axes.Right` | `bool` | Whether the right face is included. |
| `Axes.Back` | `bool` | Whether the back face is included. |
| `Axes.Front` | `bool` | Whether the front face is included. |

## API Usage (1 locations)

### Used as Property Type

- `Class.ArcHandles.Axes`
