---
title: Mouse
type: class
superclass: Instance
tags: [NotCreatable]
---

# Mouse

Legacy object that contains members useful for pointer input.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

**Mouse** has been superseded by `Class.UserInputService` and
`Class.ContextActionService`, which cover a broader scope, are more feature
rich, and support **cross-platform** patterns better. It remains supported
because of its widespread use, but you should strongly consider using these
alternatives.

The **Mouse** object houses various API for pointers, primarily for buttons
and raycasting. It can be accessed through `Class.Player:GetMouse()` called on
the `Class.Players.LocalPlayer` in a `Class.LocalScript`. It is also passed by
the `Class.Tool.Equipped` event.

- It is most notable for the `Class.Mouse.Icon|Icon` property, which changes
  the cursor's appearance.
- It continually raycasts the screen mouse position into the 3D world using
  the `Class.Mouse.TargetFilter|TargetFilter` property, storing the results of
  the raycast in the `Class.Mouse.Hit|Hit`, `Class.Mouse.Target|Target`, and
  `Class.Mouse.TargetSurface|TargetSurface` properties. These can be useful
  for simple cases, but `Class.WorldRoot:Raycast()` should be used in more
  complicated [raycasting](../../../workspace/raycasting.md) scenarios.
- `Class.Plugin|Plugins` can use `Class.Plugin:GetMouse()` to get a
  `Class.PluginMouse`, which behaves similarly.

```lua
-- From a LocalScript:
local Players = game:GetService("Players")
local player = Players.LocalPlayer
local mouse = player:GetMouse()
-- Setting the mouse icon
mouse.Icon = "rbxasset://SystemCursors/Wait"
```

Note:

- This object does not control/restrict pointer movement. For this, see
  `Class.UserInputService.MouseBehavior` and
  `Class.UserInputService.MouseDeltaSensitivity`.
- If two functions are connected to same input event, such as
  `Class.Mouse.Button1Down|Button1Down`, **both** functions will run when the
  event fires. There is no concept of sinking/passing input, as events don't
  support this behavior. However, `Class.ContextActionService` does have this
  behavior through `Class.ContextActionService:BindAction()|BindAction`.
- While a mouse may not be available on all platforms, Mouse will still
  function on mobile (touch) and console (gamepad), which don't typically have
  mice or pointer hardware. For explicit cross-platform behaviors, use
  `Class.UserInputService` and `Class.ContextActionService`.

  See [Input and Camera](../../../input/index.md) for more information on
  customizing inputs in your experience.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Mouse.Hit` | `Datatype.CFrame` | [ReadOnly] [NotReplicated] |
| `Class.Mouse.Icon` | `Datatype.ContentId` |  |
| `Class.Mouse.IconContent` | `Datatype.Content` |  |
| `Class.Mouse.Origin` | `Datatype.CFrame` | [ReadOnly] [NotReplicated] |
| `Class.Mouse.Target` | `Class.BasePart` | [ReadOnly] [NotReplicated] |
| `Class.Mouse.TargetFilter` | `Class.Instance` |  |
| `Class.Mouse.TargetSurface` | `Enum.NormalId` | [ReadOnly] [NotReplicated] |
| `Class.Mouse.UnitRay` | `Datatype.Ray` | [ReadOnly] [NotReplicated] |
| `Class.Mouse.ViewSizeX` | `int` | [ReadOnly] [NotReplicated] |
| `Class.Mouse.ViewSizeY` | `int` | [ReadOnly] [NotReplicated] |
| `Class.Mouse.X` | `int` | [ReadOnly] [NotReplicated] |
| `Class.Mouse.Y` | `int` | [ReadOnly] [NotReplicated] |
| `Class.Mouse.hit` | `Datatype.CFrame` | [Hidden] [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.Mouse.target` | `Class.BasePart` | [ReadOnly] [NotReplicated] [Deprecated] |

## Events

### `Class.Mouse.Button1Down`

Fires with: ()

### `Class.Mouse.Button1Up`

Fires with: ()

### `Class.Mouse.Button2Down`

Fires with: ()

### `Class.Mouse.Button2Up`

Fires with: ()

### `Class.Mouse.Idle`

Fires with: ()

### `Class.Mouse.KeyDown`

Fires with: (key: `string`)
  [Deprecated]

### `Class.Mouse.KeyUp`

Fires with: (key: `string`)
  [Deprecated]

### `Class.Mouse.Move`

Fires with: ()

### `Class.Mouse.WheelBackward`

Fires with: ()

### `Class.Mouse.WheelForward`

Fires with: ()

### `Class.Mouse.keyDown`

Fires with: (key: `string`)
  [Deprecated]
