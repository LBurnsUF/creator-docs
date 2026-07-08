---
title: Vector2
type: datatype
---

# `Datatype.Vector2`

Represents a 2D value with direction and magnitude.

## Description

The `Datatype.Vector2` data type represents a 2D value with direction and
magnitude. Some applications include GUI elements and 2D mouse positions.

#### Math Operations

The following math operations are valid for the `Datatype.Vector2` data type:

<table>
  <thead>
    <tr>
      <td>Operation</td>
      <td>Description</td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>Datatype.Vector2</code>&nbsp;<code>+</code>&nbsp;<code>Datatype.Vector2</code></td>
      <td>Produces a <code>Datatype.Vector2</code> with each component of the second added to the corresponding component of the first.</td>
    </tr>
    <tr>
      <td><code>Datatype.Vector2</code>&nbsp;<code>-</code>&nbsp;<code>Datatype.Vector2</code></td>
      <td>Produces a <code>Datatype.Vector2</code> with each component of the second subtracted from the corresponding component of the first.</td>
    </tr>
    <tr>
      <td><code>Datatype.Vector2</code>&nbsp;<code>*</code>&nbsp;<code>Datatype.Vector2</code></td>
      <td>Produces a <code>Datatype.Vector2</code> with each component of the second multiplied by the corresponding component of the first.</td>
    </tr>
    <tr>
      <td><code>Datatype.Vector2</code>&nbsp;<code>/</code>&nbsp;<code>Datatype.Vector2</code></td>
      <td>Produces a <code>Datatype.Vector2</code> with each component of the first divided by the corresponding component of the second.</td>
    </tr>
    <tr>
      <td><code>Datatype.Vector2</code>&nbsp;<code>*</code>&nbsp;<code>number</code></td>
      <td>Produces a <code>Datatype.Vector2</code> with each component multiplied by the number.</td>
    </tr>
    <tr>
      <td><code>Datatype.Vector2</code>&nbsp;<code>/</code>&nbsp;<code>number</code></td>
      <td>Produces a <code>Datatype.Vector2</code> with each component divided by the number.</td>
    </tr>
  </tbody>
</table>

## Constructors

### `Vector2.new`

Returns a `Datatype.Vector2` from the given x and y components.

**Parameters:**

- `x`: `number`
- `y`: `number`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Vector2.X` | `number` | The x-coordinate of the `Datatype.Vector2`. |
| `Vector2.Y` | `number` | The y-coordinate of the `Datatype.Vector2`. |
| `Vector2.Magnitude` | `number` | The length of the `Datatype.Vector2`. |
| `Vector2.Unit` | `Vector2` | A normalized copy of the `Datatype.Vector2`. |

## Methods

### `Vector2:Cross`

Returns the cross product of the two vectors.

**Parameters:**

- `other`: `Vector2`

### `Vector2:Abs`

Returns a new vector from the absolute values of the original's
components. For example, a vector of `(-2, 4)` returns a vector of
`(2, 4)`.

### `Vector2:Ceil`

Returns a new vector from the ceiling of the original's components. For
example, a vector of `(-2.6, 5.1)` returns a vector of `(-2, 6)`.

### `Vector2:Floor`

Returns a new vector from the floor of the original's components. For
example, a vector of `(-2.6, 5.1)` returns a vector of `(-3, 5)`.

### `Vector2:Sign`

Returns a new vector from the sign (-1, 0, or 1) of the original's
components. For example, a vector of `(-2.6, 5.1)` returns a vector of
`(-1, 1)`.

### `Vector2:Angle`

Returns the angle in radians between the two vectors. Specify `true` for
the optional `isSigned` boolean if you want a signed angle. By default,
the method returns the absolute value. Signed angles are a negative when
going clockwise. Values are in the range `[0, pi]` for absolute angles and
`[-pi, pi]` for signed angles.

**Parameters:**

- `other`: `Vector2`
- `isSigned`: `boolean`

### `Vector2:Dot`

Returns a scalar dot product of the two vectors.

**Parameters:**

- `v`: `Vector2`

### `Vector2:Lerp`

Returns a `Datatype.Vector2` linearly interpolated between this
`Datatype.Vector2` and the given goal by the given alpha.

**Parameters:**

- `v`: `Vector2`
- `alpha`: `number`

### `Vector2:Max`

Returns a `Datatype.Vector2` with each component as the highest among the
respective components of the provided `Datatype.Vector2` objects.

```lua
local a = Vector2.new(1, 2)
local b = Vector2.new(2, 1)

print(a:Max(b)) -- Vector2.new(2, 2)
```

**Parameters:**

- `others...`: `Tuple`

### `Vector2:Min`

Returns a `Datatype.Vector2` with each component as the lowest among the
respective components of the provided `Datatype.Vector2` objects.

```lua
local a = Vector2.new(1, 2)
local b = Vector2.new(2, 1)

print(a:Min(b)) -- Vector2.new(1, 1)
```

**Parameters:**

- `others...`: `Tuple`

### `Vector2:FuzzyEq`

Returns `true` if the X and Y components of the other `Datatype.Vector2`
are within epsilon units of each corresponding component of this
`Datatype.Vector2`.

**Parameters:**

- `other`: `Vector2`
- `epsilon`: `number`

## Math Operations

| Operation | Description |
|-----------|-------------|
| `Vector2` + | Produces a `Datatype.Vector2` with each component of the second added to the corresponding component |
| `Vector2` - | Produces a `Datatype.Vector2` with each component of the second subtracted from the corresponding co |
| `Vector2` * | Produces a `Datatype.Vector2` with each component of the second multiplied by the corresponding comp |
| `Vector2` / | Produces a `Datatype.Vector2` with each component of the first divided by the corresponding componen |
| `Vector2` * | Produces a `Datatype.Vector2` with each component multiplied by the number. |
| `Vector2` / | Produces a `Datatype.Vector2` with each component divided by the number. |

## API Usage (146 locations)

### Used as Property Type

- `Class.BillboardGui.SizeOffset`
- `Class.Camera.ViewportSize`
- `Class.ChannelTabsConfiguration.AbsolutePosition`
- `Class.ChannelTabsConfiguration.AbsoluteSize`
- `Class.ChatInputBarConfiguration.AbsolutePosition`
- `Class.ChatInputBarConfiguration.AbsolutePositionWrite`
- `Class.ChatInputBarConfiguration.AbsoluteSize`
- `Class.ChatInputBarConfiguration.AbsoluteSizeWrite`
- `Class.ChatWindowConfiguration.AbsolutePosition`
- `Class.ChatWindowConfiguration.AbsolutePositionWrite`
- `Class.ChatWindowConfiguration.AbsoluteSize`
- `Class.ChatWindowConfiguration.AbsoluteSizeWrite`
- `Class.Decal.UVOffset`
- `Class.Decal.UVScale`
- `Class.EditableImage.Size`
- `Class.ExplorerFilterAutocompleter.ReplaceRange`
- `Class.FloorWire.TextureSize`
- `Class.GuiBase2d.AbsolutePosition`
- `Class.GuiBase2d.AbsoluteSize`
- `Class.GuiObject.AnchorPoint`
- `Class.GuiService.ViewportSizeInMM`
- `Class.ImageButton.ContentImageSize`
- `Class.ImageButton.ImageRectOffset`
- `Class.ImageButton.ImageRectSize`
- `Class.ImageHandleAdornment.Size`
- `Class.ImageLabel.ContentImageSize`
- `Class.ImageLabel.ImageRectOffset`
- `Class.ImageLabel.ImageRectSize`
- `Class.InputAction.Direction2DState`
- `Class.InputAction.ViewportPositionState`
- `Class.InputBinding.Vector2Scale`
- `Class.LinearVelocity.MaxPlanarAxesForce`
- `Class.LinearVelocity.PlaneVelocity`
- `Class.ParticleEmitter.SpreadAngle`
- `Class.PluginDragEvent.Position`
- `Class.ProximityPrompt.UIOffset`
- `Class.ScrollingFrame.AbsoluteCanvasSize`
- `Class.ScrollingFrame.AbsoluteWindowSize`
- `Class.ScrollingFrame.CanvasPosition`
- `Class.ScrollingFrame.MaxCanvasPosition`
- ...and 38 more

### Used as Parameter Type

- `Class.BasePlayerGui:GetGuiObjectsInCircle` (parameter `position`)
- `Class.ChannelTabsConfiguration:SetAbsolutePosition` (parameter `value`)
- `Class.ChannelTabsConfiguration:SetAbsoluteSize` (parameter `value`)
- `Class.EditableImage:DrawCircle` (parameter `center`)
- `Class.EditableImage:DrawImage` (parameter `position`)
- `Class.EditableImage:DrawImageTransformed` (parameter `position`)
- `Class.EditableImage:DrawImageTransformed` (parameter `scale`)
- `Class.EditableImage:DrawLine` (parameter `p1`)
- `Class.EditableImage:DrawLine` (parameter `p2`)
- `Class.EditableImage:DrawRectangle` (parameter `position`)
- `Class.EditableImage:DrawRectangle` (parameter `size`)
- `Class.EditableImage:DrawTriangle` (parameter `p1`)
- `Class.EditableImage:DrawTriangle` (parameter `p2`)
- `Class.EditableImage:DrawTriangle` (parameter `p3`)
- `Class.EditableImage:ReadPixelsBuffer` (parameter `position`)
- `Class.EditableImage:ReadPixelsBuffer` (parameter `size`)
- `Class.EditableImage:WritePixelsBuffer` (parameter `position`)
- `Class.EditableImage:WritePixelsBuffer` (parameter `size`)
- `Class.EditableMesh:AddUV` (parameter `uv`)
- `Class.EditableMesh:SetUV` (parameter `uv`)
- `Class.GamepadService:GamepadThumbstick1Changed` (parameter `event`)
- `Class.GamepadService:SetGamepadCursorPosition` (parameter `position`)
- `Class.GuiObject:TouchPan` (parameter `totalTranslation`)
- `Class.GuiObject:TouchPan` (parameter `velocity`)
- `Class.PluginGui:PointerAction` (parameter `pan`)
- `Class.StudioDeviceEmulatorService:EmulatePCDeviceWithResolution` (parameter `resolution`)
- `Class.StudioScreenshotCapture:ScaleAsync` (parameter `newSize`)
- `Class.TextService:GetTextSize` (parameter `frameSize`)
- `Class.UIDragDetector:DragContinue` (parameter `inputPosition`)
- `Class.UIDragDetector:DragEnd` (parameter `inputPosition`)
- `Class.UIDragDetector:DragStart` (parameter `inputPosition`)
- `Class.UserInputService:PointerAction` (parameter `pan`)
- `Class.UserInputService:SendAppUISizes` (parameter `bottomBarSize`)
- `Class.UserInputService:SendAppUISizes` (parameter `navBarSize`)
- `Class.UserInputService:SendAppUISizes` (parameter `rightBarSize`)
- `Class.UserInputService:SendAppUISizes` (parameter `statusBarSize`)
- `Class.UserInputService:StatusBarTapped` (parameter `position`)
- `Class.UserInputService:TouchPan` (parameter `totalTranslation`)
- `Class.UserInputService:TouchPan` (parameter `velocity`)
- `Class.UserInputService:TouchTapInWorld` (parameter `position`)
- ...and 11 more

### Used as Return Type

- `Class.CaptureService:GetCaptureSizeAsync`
- `Class.EditableMesh:GetUV`
- `Class.GamepadService:GetGamepadCursorPosition`
- `Class.GuiService:GetHardwareSafeViewport`
- `Class.GuiService:GetScreenResolution`
- `Class.Path2D:GetTangentOnCurve`
- `Class.Path2D:GetTangentOnCurveArcLength`
- `Class.PluginGui:GetRelativeMousePosition`
- `Class.ScrollingFrame:GetSampledInertialVelocity`
- `Class.ScrollingFrame:GetScrollVelocity`
- `Class.StudioDeviceEmulatorService:GetTouchPosition`
- `Class.StudioDeviceSimulatorService:GetResolutionAsync`
- `Class.TextService:GetTextBoundsAsync`
- `Class.TextService:GetTextSize`
- `Class.UGCValidationService:GetEditableImageSize`
- `Class.UserInputService:GetMouseDelta`
- `Class.UserInputService:GetMouseLocation`
