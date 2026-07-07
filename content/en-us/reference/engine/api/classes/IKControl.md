---
title: IKControl
type: class
superclass: Instance
---

# IKControl

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.IKControl.ChainRoot` | `Class.Instance` |  |
| `Class.IKControl.Enabled` | `bool` |  |
| `Class.IKControl.EndEffector` | `Class.Instance` |  |
| `Class.IKControl.EndEffectorOffset` | `Datatype.CFrame` |  |
| `Class.IKControl.Offset` | `Datatype.CFrame` |  |
| `Class.IKControl.Pole` | `Class.Instance` |  |
| `Class.IKControl.Priority` | `int` |  |
| `Class.IKControl.SmoothTime` | `float` |  |
| `Class.IKControl.Target` | `Class.Instance` |  |
| `Class.IKControl.Type` | `Enum.IKControlType` |  |
| `Class.IKControl.Weight` | `float` |  |

## Methods

### `Class.IKControl:GetChainCount`

``GetChainCount()`` → `int`

### `Class.IKControl:GetChainLength`

``GetChainLength()`` → `float`

### `Class.IKControl:GetNodeLocalCFrame`

``GetNodeLocalCFrame(index: `int`)`` → `Datatype.CFrame`

### `Class.IKControl:GetNodeWorldCFrame`

``GetNodeWorldCFrame(index: `int`)`` → `Datatype.CFrame`

### `Class.IKControl:GetRawFinalTarget`

``GetRawFinalTarget()`` → `Datatype.CFrame`

### `Class.IKControl:GetSmoothedFinalTarget`

``GetSmoothedFinalTarget()`` → `Datatype.CFrame`

### `Class.IKControl:Solve`

``Solve()`` → `null`
   {security: RobloxScriptSecurity}
