---
title: InputAction
type: class
superclass: Instance
---

# InputAction

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.InputAction.BoolState` | `bool` | [ReadOnly] [NotReplicated] [NotScriptable] {security: RobloxScriptSecurity} |
| `Class.InputAction.Direction1DState` | `float` | [ReadOnly] [NotReplicated] [NotScriptable] {security: RobloxScriptSecurity} |
| `Class.InputAction.Direction2DState` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] [NotScriptable] {security: RobloxScriptSecurity} |
| `Class.InputAction.Direction3DState` | `Datatype.Vector3` | [ReadOnly] [NotReplicated] [NotScriptable] {security: RobloxScriptSecurity} |
| `Class.InputAction.Enabled` | `bool` |  |
| `Class.InputAction.Type` | `Enum.InputActionType` |  |
| `Class.InputAction.ViewportPositionState` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] [NotScriptable] {security: RobloxScriptSecurity} |

## Methods

### `Class.InputAction:Fire`

``Fire(state: `Variant`)`` → `null`
  [Deprecated]

### `Class.InputAction:GetInputBindings`

``GetInputBindings()`` → `Datatype.Instances`
   {security: RobloxScriptSecurity}

### `Class.InputAction:GetState`

``GetState()`` → `Variant`

## Events

### `Class.InputAction.InputBindingsChanged`

Fires with: ()

### `Class.InputAction.Pressed`

Fires with: ()

### `Class.InputAction.Released`

Fires with: ()

### `Class.InputAction.StateChanged`

Fires with: (value: `Variant`)
