---
title: VideoDisplay
type: class
superclass: GuiObject
---

# VideoDisplay

**Inherits from:** `Class.GuiObject` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.VideoDisplay.ResampleMode` | `Enum.ResamplerMode` |  |
| `Class.VideoDisplay.ScaleType` | `Enum.ScaleType` |  |
| `Class.VideoDisplay.TileSize` | `Datatype.UDim2` |  |
| `Class.VideoDisplay.VideoColor3` | `Datatype.Color3` |  |
| `Class.VideoDisplay.VideoRectOffset` | `Datatype.Vector2` |  |
| `Class.VideoDisplay.VideoRectSize` | `Datatype.Vector2` |  |
| `Class.VideoDisplay.VideoTransparency` | `float` |  |

## Methods

### `Class.VideoDisplay:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` → `Datatype.Instances`

### `Class.VideoDisplay:GetInputPins`

``GetInputPins()`` → `Array`

### `Class.VideoDisplay:GetOutputPins`

``GetOutputPins()`` → `Array`

## Events

### `Class.VideoDisplay.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)
