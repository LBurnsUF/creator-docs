---
title: ViewportFrame
type: class
superclass: GuiObject
---

# ViewportFrame

`Class.GuiObject` that renders 3D objects inside its bounds.

**Inherits from:** `Class.GuiObject` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Description

`ViewportFrame` is a `Class.GuiObject` that renders 3D objects inside its
bounds, offering a way to display 3D objects in a 2D space like a
`Class.ScreenGui`. This object has the following caveats:

- No shadows or
  [post-processing](../../../environment/post-processing-effects.md) effects
  are rendered.

- `Enum.Material.Neon` and `Enum.Material.Glass` materials render at the
  lowest quality.

- Nested `Class.GuiObject|GuiObjects` aren't supported.

- By default, lighting inside a `ViewportFrame` acts as if
  `Class.Lighting.EnvironmentSpecularScale` and
  `Class.Lighting.EnvironmentDiffuseScale` are both set to `0`, so properties
  that rely on these fields, such as `Class.SurfaceAppearance.MetalnessMap`,
  may look different.

- This object can use a `Class.Sky` child as a cubemap for reflections, in
  which case only the `Class.Sky` object's six `Skybox[…]` properties are
  used. Assuming these properties are valid, lighting inside the
  `ViewportFrame` acts similarly to if
  `Class.Lighting.EnvironmentSpecularScale` and
  `Class.Lighting.EnvironmentDiffuseScale` are both set to `1`. For details,
  see [here](../../../ui/viewport-frames.md).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ViewportFrame.Ambient` | `Datatype.Color3` |  |
| `Class.ViewportFrame.CurrentCamera` | `Class.Camera` | [NotReplicated] |
| `Class.ViewportFrame.ImageColor3` | `Datatype.Color3` |  |
| `Class.ViewportFrame.ImageTransparency` | `float` |  |
| `Class.ViewportFrame.IsMirrored` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.ViewportFrame.LightColor` | `Datatype.Color3` |  |
| `Class.ViewportFrame.LightDirection` | `Datatype.Vector3` |  |

## Methods

### `Class.ViewportFrame:CaptureSnapshotAsync`

``CaptureSnapshotAsync()`` -> `Datatype.ContentId`
  [Yields] {security: RobloxScriptSecurity}
