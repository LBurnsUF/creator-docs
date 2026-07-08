---
title: VideoDisplay
type: class
superclass: GuiObject
---

# VideoDisplay

A GUI object that displays video content from a connected `Class.VideoPlayer`.

**Inherits from:** `Class.GuiObject` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Description

A `Class.VideoDisplay` is a GUI object that displays video content from a
`Class.VideoPlayer` connected via a `Class.Wire`. It functions similarly to a
`Class.ImageLabel` but is designed for video playback.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.VideoDisplay.ResampleMode` | `Enum.ResamplerMode` |  |
| `Class.VideoDisplay.ScaleType` | `Enum.ScaleType` |  |
| `Class.VideoDisplay.TileSize` | `Datatype.UDim2` |  |
| `Class.VideoDisplay.VideoColor3` | `Datatype.Color3` |  |
| `Class.VideoDisplay.VideoRectOffset` | `Datatype.Vector2` |  |
| `Class.VideoDisplay.VideoRectSize` | `Datatype.Vector2` |  |
| `Class.VideoDisplay.VideoTransparency` | `float` |  |

## Methods

### `Class.VideoDisplay:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.VideoDisplay:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.VideoDisplay:GetOutputPins`

``GetOutputPins()`` -> `Array`

## Events

### `Class.VideoDisplay.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)
