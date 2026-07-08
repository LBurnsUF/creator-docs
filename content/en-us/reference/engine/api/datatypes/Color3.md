---
title: Color3
type: datatype
---

# `Datatype.Color3`

A color value comprised of red, green, and blue components.

## Description

The `Datatype.Color3` data type describes a color using red, green, and blue
components in the range of 0 to 1. Unlike the `Datatype.BrickColor` data type
which describes named colors, `Datatype.Color3` is used for precise coloring
of objects on screen through properties like `Class.BasePart.Color` and
`Class.GuiObject.BackgroundColor3`.

## Constructors

### `Color3.new`

Returns a `Datatype.Color3` with the given red, green, and blue values.
The parameters should be within the range of 0 to 1.

```lua
local red = Color3.new(1, 0, 0)
local green = Color3.new(0, 1, 0)
local blue = Color3.new(0, 0, 1)
```

**Parameters:**

- `red`: `number`
- `green`: `number`
- `blue`: `number`

### `Color3.fromRGB`

Creates a `Datatype.Color3` with the given red, green, and blue
components. Unlike most other `Datatype.Color3` functions, the parameters
for this function should be within the range of 0 to 255.

```lua
local red = Color3.fromRGB(255, 0, 0)
local green = Color3.fromRGB(0, 255, 0)
local blue = Color3.fromRGB(0, 0, 255)
```

**Parameters:**

- `red`: `number`
- `green`: `number`
- `blue`: `number`

### `Color3.fromHSV`

Creates a `Datatype.Color3` with the given hue, saturation, and value. The
parameters should be within the range of 0 to 1.

```lua
local red = Color3.fromHSV(1, 1, 1)
local green = Color3.fromHSV(0.3333333, 1, 1)
local white = Color3.fromHSV(0, 0, 1)
```

**Parameters:**

- `hue`: `number`
- `saturation`: `number`
- `value`: `number`

### `Color3.fromHex`

Returns a new `Datatype.Color3` from a six- or three-character hexadecimal
format, case insensitive. A preceding hashtag (`#`) is ignored, if
present. This function interprets the given string as a typical web hex
color in the format `RRGGBB` or `RGB` (shorthand for `RRGGBB`). For
example, `#FFAA00` produces an orange color and is the same as `#FA0`.

```lua
local red = Color3.fromHex("FF0000")
local magenta = Color3.fromHex("ec008c")
local black = Color3.fromHex("000")
local white = Color3.fromHex("#FFF")
```

**Parameters:**

- `hex`: `string`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Color3.R` | `number` | The red value of the color. |
| `Color3.G` | `number` | The green value of the color. |
| `Color3.B` | `number` | The blue value of the color. |

## Methods

### `Color3:Lerp`

Returns a `Datatype.Color3` interpolated between two colors. The `alpha`
value should be within the range of 0 to 1.

```lua
local white = Color3.new(1, 1, 1)
local black = Color3.new(0, 0, 0)

local gray10 = white:Lerp(black, 0.1)
print(gray10)  --> 0.9, 0.9, 0.9

local gray50 = white:Lerp(black, 0.5)
print(gray50)  --> 0.5, 0.5, 0.5

local gray85 = white:Lerp(black, 0.85)
print(gray85)  --> 0.15, 0.15, 0.15
```

**Parameters:**

- `color`: `Color3`
- `alpha`: `number`

### `Color3:ToHSV`

Returns the hue, saturation, and value of a `Datatype.Color3`. This
function is the inverse operation of the `Datatype.Color3.fromHSV()`
constructor.

```lua
local red = Color3.fromRGB(255, 0, 0)
local green = Color3.fromRGB(0, 255, 0)

local redH, redS, redV = red:ToHSV()
print(redH, redS, redV)  --> 1 1 1

local greenH, greenS, greenV = green:ToHSV()
print(greenH, greenS, greenV)  --> 0.3333333 1 1
```

### `Color3:ToHex`

Converts the color to a six-character hexadecimal string representing the
color in the format `RRGGBB`. It is not prefixed with an octothorpe (`#`).

The returned string can be provided to `Datatype.Color3.fromHex()` to
produce the original color.

```lua
local red = Color3.fromRGB(255, 0, 0)
local magenta = Color3.fromRGB(236, 0, 140)

local redHex = red:ToHex()
print(redHex)  --> ff0000

local magentaHex = magenta:ToHex()
print(magentaHex)  --> ec008c
```

## API Usage (155 locations)

### Used as Property Type

- `Class.Annotation.AuthorColor3`
- `Class.Atmosphere.Color`
- `Class.Atmosphere.Decay`
- `Class.BasePart.Color`
- `Class.BodyColors.HeadColor3`
- `Class.BodyColors.LeftArmColor3`
- `Class.BodyColors.LeftLegColor3`
- `Class.BodyColors.RightArmColor3`
- `Class.BodyColors.RightLegColor3`
- `Class.BodyColors.TorsoColor3`
- `Class.BodyPartDescription.Color`
- `Class.BubbleChatConfiguration.BackgroundColor3`
- `Class.BubbleChatConfiguration.TextColor3`
- `Class.BubbleChatMessageProperties.BackgroundColor3`
- `Class.BubbleChatMessageProperties.TextColor3`
- `Class.CanvasGroup.GroupColor3`
- `Class.ChannelTabsConfiguration.BackgroundColor3`
- `Class.ChannelTabsConfiguration.HoverBackgroundColor3`
- `Class.ChannelTabsConfiguration.SelectedTabTextColor3`
- `Class.ChannelTabsConfiguration.TextColor3`
- `Class.ChannelTabsConfiguration.TextStrokeColor3`
- `Class.ChatInputBarConfiguration.BackgroundColor3`
- `Class.ChatInputBarConfiguration.PlaceholderColor3`
- `Class.ChatInputBarConfiguration.TextColor3`
- `Class.ChatInputBarConfiguration.TextStrokeColor3`
- `Class.ChatWindowConfiguration.BackgroundColor3`
- `Class.ChatWindowConfiguration.TextColor3`
- `Class.ChatWindowConfiguration.TextStrokeColor3`
- `Class.ChatWindowMessageProperties.TextColor3`
- `Class.ChatWindowMessageProperties.TextStrokeColor3`
- `Class.Clothing.Color3`
- `Class.Clouds.Color`
- `Class.Collaborator.CollaboratorColor3`
- `Class.Color3Value.Value`
- `Class.ColorCorrectionEffect.TintColor`
- `Class.Decal.Color3`
- `Class.DraggerService.GeometrySnapColor`
- `Class.Fire.Color`
- `Class.Fire.SecondaryColor`
- `Class.GuiBase3d.Color3`
- ...and 102 more

### Used as Parameter Type

- `Class.Color3Value:Changed` (parameter `value`)
- `Class.Color3Value:changed` (parameter `value`)
- `Class.EditableImage:DrawCircle` (parameter `color`)
- `Class.EditableImage:DrawLine` (parameter `color`)
- `Class.EditableImage:DrawRectangle` (parameter `color`)
- `Class.EditableImage:DrawTriangle` (parameter `color`)
- `Class.EditableMesh:AddColor` (parameter `color`)
- `Class.EditableMesh:SetColor` (parameter `color`)
- `Class.Terrain:SetMaterialColor` (parameter `value`)
- `Class.Terrain:SetMaterialSlot` (parameter `color`)

### Used as Return Type

- `Class.EditableMesh:GetColor`
- `Class.StudioTheme:GetColor`
- `Class.Terrain:GetMaterialColor`
