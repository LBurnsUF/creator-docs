---
title: VideoDisplay
type: class
superclass: GuiObject
---

# VideoDisplay

**Inherits**: GuiObject > GuiBase2d > GuiBase > Instance > Object

## Properties

- **ResampleMode**: `ResamplerMode`
- **ScaleType**: `ScaleType`
- **TileSize**: `UDim2`
- **VideoColor3**: `Color3`
- **VideoRectOffset**: `Vector2`
- **VideoRectSize**: `Vector2`
- **VideoTransparency**: `float`

## Methods

- **GetConnectedWires**(`pin: string`) -> `Instances`
- **GetInputPins**() -> `Array`
- **GetOutputPins**() -> `Array`

## Events

- **WiringChanged**(`connected: bool`, `pin: string`, `wire: Wire`, `instance: Instance`)
