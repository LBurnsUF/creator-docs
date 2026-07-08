---
title: MarkerCurve
type: class
superclass: Instance
---

# MarkerCurve

Represents a list of strings markers in chronological order.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

The MarkerCurve instance lets you place markers as string values at certain
times on a timeline. The string at each marker cannot exceed 64 characters and
must only contain printable characters.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.MarkerCurve.Length` | `int` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.MarkerCurve:GetMarkerAtIndex`

``GetMarkerAtIndex(index: `int`)`` -> `Dictionary`

### `Class.MarkerCurve:GetMarkers`

``GetMarkers()`` -> `Array`

### `Class.MarkerCurve:InsertMarkerAtTime`

``InsertMarkerAtTime(time: `float`, marker: `string`)`` -> `Array`

### `Class.MarkerCurve:RemoveMarkerAtIndex`

``RemoveMarkerAtIndex(startingIndex: `int`, count: `int`)`` -> `int`
