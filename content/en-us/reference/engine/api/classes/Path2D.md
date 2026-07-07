---
title: Path2D
type: class
superclass: GuiBase
---

# Path2D

**Inherits**: GuiBase > Instance > Object

## Properties

- **Closed**: `bool`
- **Color3**: `Color3`
- **SelectedControlPoint**: `int` [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **SelectedControlPointData**: `Path2DControlPoint` [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Thickness**: `float`
- **Transparency**: `float` (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Visible**: `bool`
- **ZIndex**: `int`

## Methods

- **GetBoundingRect**() -> `Rect`
- **GetControlPoint**(`index: int`) -> `Path2DControlPoint`
- **GetControlPoints**() -> `Array`
- **GetLength**() -> `float`
- **GetMaxControlPoints**() -> `int`
- **GetPositionOnCurve**(`t: float`) -> `UDim2`
- **GetPositionOnCurveArcLength**(`t: float`) -> `UDim2`
- **GetSegmentCount**() -> `int`
- **GetTangentOnCurve**(`t: float`) -> `Vector2`
- **GetTangentOnCurveArcLength**(`t: float`) -> `Vector2`
- **InsertControlPoint**(`index: int`, `point: Path2DControlPoint`) -> `null`
- **RemoveControlPoint**(`index: int`) -> `null`
- **SetControlPoints**(`controlPoints: Array`) -> `null`
- **UpdateControlPoint**(`index: int`, `point: Path2DControlPoint`) -> `null`

## Events

- **ControlPointChanged**()
