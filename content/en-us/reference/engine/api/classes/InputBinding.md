---
title: InputBinding
type: class
superclass: Instance
---

# InputBinding

Defines which hardware binding should trigger the parent `Class.InputAction`.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

An `InputBinding` defines which hardware binding should trigger the parent
`Class.InputAction`, for example a key press, gamepad button, or tap on a
touch‑enabled device. There can be multiple `InputBinding` instances parented
to an `Class.InputAction`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.InputBinding.Backward` | `Enum.KeyCode` |  |
| `Class.InputBinding.ClampMagnitudeToOne` | `bool` |  |
| `Class.InputBinding.Down` | `Enum.KeyCode` |  |
| `Class.InputBinding.Forward` | `Enum.KeyCode` |  |
| `Class.InputBinding.KeyCode` | `Enum.KeyCode` |  |
| `Class.InputBinding.Left` | `Enum.KeyCode` |  |
| `Class.InputBinding.PointerIndex` | `int` |  |
| `Class.InputBinding.PressedThreshold` | `float` |  |
| `Class.InputBinding.PrimaryModifier` | `Enum.KeyCode` |  |
| `Class.InputBinding.ReleasedThreshold` | `float` |  |
| `Class.InputBinding.ResponseCurve` | `float` |  |
| `Class.InputBinding.Right` | `Enum.KeyCode` |  |
| `Class.InputBinding.Scale` | `float` |  |
| `Class.InputBinding.SecondaryModifier` | `Enum.KeyCode` |  |
| `Class.InputBinding.Type` | `Enum.InputBindingType` |  |
| `Class.InputBinding.UIButton` | `Class.GuiButton` |  |
| `Class.InputBinding.UIModifier` | `Class.GuiButton` |  |
| `Class.InputBinding.Up` | `Enum.KeyCode` |  |
| `Class.InputBinding.Vector2Scale` | `Datatype.Vector2` |  |
| `Class.InputBinding.Vector3Scale` | `Datatype.Vector3` |  |

## Methods

### `Class.InputBinding:Fire`

``Fire(state: `Variant`)`` -> `null`
