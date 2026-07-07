---
title: Path2D
type: class
superclass: GuiBase
---

# Path2D

**Inherits from:** `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.Path2D.Closed` | `bool` |  |
| `Class.Path2D.Color3` | `Datatype.Color3` |  |
| `Class.Path2D.SelectedControlPoint` | `int` | [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Path2D.SelectedControlPointData` | `Datatype.Path2DControlPoint` | [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Path2D.Thickness` | `float` |  |
| `Class.Path2D.Transparency` | `float` |  {security: RobloxScriptSecurity} |
| `Class.Path2D.Visible` | `bool` |  |
| `Class.Path2D.ZIndex` | `int` |  |

## Methods

### `Class.Path2D:GetBoundingRect`

``GetBoundingRect()`` → `Datatype.Rect`

### `Class.Path2D:GetControlPoint`

``GetControlPoint(index: `int`)`` → `Datatype.Path2DControlPoint`

### `Class.Path2D:GetControlPoints`

``GetControlPoints()`` → `Array`

### `Class.Path2D:GetLength`

``GetLength()`` → `float`

### `Class.Path2D:GetMaxControlPoints`

``GetMaxControlPoints()`` → `int`

### `Class.Path2D:GetPositionOnCurve`

``GetPositionOnCurve(t: `float`)`` → `Datatype.UDim2`

### `Class.Path2D:GetPositionOnCurveArcLength`

``GetPositionOnCurveArcLength(t: `float`)`` → `Datatype.UDim2`

### `Class.Path2D:GetSegmentCount`

``GetSegmentCount()`` → `int`
   {security: RobloxScriptSecurity}

### `Class.Path2D:GetTangentOnCurve`

``GetTangentOnCurve(t: `float`)`` → `Datatype.Vector2`

### `Class.Path2D:GetTangentOnCurveArcLength`

``GetTangentOnCurveArcLength(t: `float`)`` → `Datatype.Vector2`

### `Class.Path2D:InsertControlPoint`

``InsertControlPoint(index: `int`, point: `Datatype.Path2DControlPoint`)`` → `null`

### `Class.Path2D:RemoveControlPoint`

``RemoveControlPoint(index: `int`)`` → `null`

### `Class.Path2D:SetControlPoints`

``SetControlPoints(controlPoints: `Array`)`` → `null`

### `Class.Path2D:UpdateControlPoint`

``UpdateControlPoint(index: `int`, point: `Datatype.Path2DControlPoint`)`` → `null`

## Events

### `Class.Path2D.ControlPointChanged`

Fires with: ()
