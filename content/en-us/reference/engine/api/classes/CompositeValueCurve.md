---
title: CompositeValueCurve
type: class
superclass: Instance
---

# CompositeValueCurve

An animation curve that groups child `Class.FloatCurve|FloatCurves` which each
animate a different component of a non-unary value.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

An animation curve that groups child `Class.FloatCurve|FloatCurves` which each
animate a different component of a non-unary value. The
`Class.CompositeValueCurve.CurveType|CurveType` property specifies the type of
value to be animated and, depending on this value, differently named children
are used to drive the animation of the components of the value.

As follows are the names of the child curves that drive the animation for each
possible `Enum.CompositeValueCurveType` value for
`Class.CompositeValueCurve.CurveType|CurveType`:

- `Enum.CompositeValueCurveType.ColorRGB|ColorRGB`: { `"R"`, `"G"`, `"B"` }
- `Enum.CompositeValueCurveType.ColorHSV|ColorHSV`: { `"H"`, `"S"`, `"V"` }
- `Enum.CompositeValueCurveType.NumberRange|NumberRange`: { `"Min"`, `"Max"` }
- `Enum.CompositeValueCurveType.Rect|Rect`: { `"MinX"`, `"MaxX"`, `"MinY"`,
  `"MaxY"` }
- `Enum.CompositeValueCurveType.UDim|UDim`: { `"Scale"`, `"Offset"` }
- `Enum.CompositeValueCurveType.UDim2|UDim2`: { `"ScaleX"`, `"OffsetX"`,
  `"ScaleY"`, `"OffsetY"` }
- `Enum.CompositeValueCurveType.Vector2|Vector2`: { `"X"`, `"Y"`}
- `Enum.CompositeValueCurveType.Vector3|Vector3`: { `"X"`, `"Y"`, `"Z"` }

The children that drive the animation can be accessed via the
`Class.CompositeValueCurve:GetComponentCurves()|GetComponentCurves()` method
which returns an array of curves in the order specified above. The value of
the curve at a given time in the animation may be sampled by the
`Class.CompositeValueCurve:GetValueAtTime()|GetValueAtTime()` method.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.CompositeValueCurve.CurveType` | `Enum.CompositeValueCurveType` |  |

## Methods

### `Class.CompositeValueCurve:GetComponentCurves`

``GetComponentCurves()`` -> `Datatype.Instances`

### `Class.CompositeValueCurve:GetValueAtTime`

``GetValueAtTime(time: `float`)`` -> `Variant`
