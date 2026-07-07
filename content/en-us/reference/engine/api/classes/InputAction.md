---
title: InputAction
type: class
superclass: Instance
---

# InputAction

**Inherits**: Instance > Object

## Properties

- **BoolState**: `bool` [ReadOnly] [NotReplicated] [NotScriptable] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Direction1DState**: `float` [ReadOnly] [NotReplicated] [NotScriptable] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Direction2DState**: `Vector2` [ReadOnly] [NotReplicated] [NotScriptable] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Direction3DState**: `Vector3` [ReadOnly] [NotReplicated] [NotScriptable] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Enabled**: `bool`
- **Type**: `InputActionType`
- **ViewportPositionState**: `Vector2` [ReadOnly] [NotReplicated] [NotScriptable] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **Fire**(`state: Variant`) -> `null` [Deprecated]
- **GetInputBindings**() -> `Instances`
- **GetState**() -> `Variant`

## Events

- **InputBindingsChanged**()
- **Pressed**()
- **Released**()
- **StateChanged**(`value: Variant`)
