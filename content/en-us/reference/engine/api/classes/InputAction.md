---
title: InputAction
type: class
superclass: Instance
---

# InputAction

Defines a gameplay action mechanic. These actions are then mapped to hardware
inputs using `Class.InputBinding`.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`InputAction` defines a gameplay action mechanic such as "Jump," "Sprint," or
"Shoot." These actions are then mapped to hardware inputs using
`Class.InputBinding`. An `InputAction` will check for its first ancestor type
of `Class.InputContext` and register itself to that context (if there is no
ancestor context, it will be registered to a default context).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.InputAction.BoolState` | `bool` | [ReadOnly] [NotReplicated] [NotScriptable] {security: RobloxScriptSecurity} |
| `Class.InputAction.Direction1DState` | `float` | [ReadOnly] [NotReplicated] [NotScriptable] {security: RobloxScriptSecurity} |
| `Class.InputAction.Direction2DState` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] [NotScriptable] {security: RobloxScriptSecurity} |
| `Class.InputAction.Direction3DState` | `Datatype.Vector3` | [ReadOnly] [NotReplicated] [NotScriptable] {security: RobloxScriptSecurity} |
| `Class.InputAction.Enabled` | `bool` |  |
| `Class.InputAction.Type` | `Enum.InputActionType` |  |
| `Class.InputAction.ViewportPositionState` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] [NotScriptable] {security: RobloxScriptSecurity} |

## Methods

### `Class.InputAction:Fire`

``Fire(state: `Variant`)`` -> `null`
  [Deprecated]

### `Class.InputAction:GetInputBindings`

``GetInputBindings()`` -> `Datatype.Instances`
   {security: RobloxScriptSecurity}

### `Class.InputAction:GetState`

``GetState()`` -> `Variant`

## Events

### `Class.InputAction.InputBindingsChanged`

Fires with: ()

### `Class.InputAction.Pressed`

Fires with: ()

### `Class.InputAction.Released`

Fires with: ()

### `Class.InputAction.StateChanged`

Fires with: (value: `Variant`)
