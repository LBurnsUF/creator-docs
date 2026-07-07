---
title: GuiObject
type: class
superclass: GuiBase2d
tags: [NotCreatable, NotBrowsable]
---

# GuiObject

**Inherits**: GuiBase2d > GuiBase > Instance > Object

**Tags**: NotCreatable, NotBrowsable

## Properties

- **Active**: `bool`
- **AnchorPoint**: `Vector2`
- **AutomaticSize**: `AutomaticSize`
- **BackgroundColor**: `BrickColor` [Hidden] [NotReplicated] [Deprecated]
- **BackgroundColor3**: `Color3`
- **BackgroundTransparency**: `float`
- **BorderColor**: `BrickColor` [Hidden] [NotReplicated] [Deprecated]
- **BorderColor3**: `Color3`
- **BorderMode**: `BorderMode`
- **BorderSizePixel**: `int`
- **ClipsDescendants**: `bool`
- **Draggable**: `bool` [Deprecated]
- **GuiState**: `GuiState` [ReadOnly] [NotReplicated]
- **InputSink**: `InputSink`
- **Interactable**: `bool`
- **LayoutOrder**: `int`
- **NextSelectionDown**: `GuiObject`
- **NextSelectionLeft**: `GuiObject`
- **NextSelectionRight**: `GuiObject`
- **NextSelectionUp**: `GuiObject`
- **Position**: `UDim2`
- **Rotation**: `float`
- **Selectable**: `bool`
- **SelectionImageObject**: `GuiObject`
- **SelectionOrder**: `int`
- **SelectionRect2D**: `Rect` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Size**: `UDim2`
- **SizeConstraint**: `SizeConstraint`
- **Transparency**: `float` [Hidden] [NotReplicated]
- **Visible**: `bool`
- **ZIndex**: `int`

## Methods

- **TweenPosition**(`endPosition: UDim2`, `easingDirection: EasingDirection = Out`, `easingStyle: EasingStyle = Quad`, `time: float = 1`, `override: bool = false`, `callback: Function = nil`) -> `bool`
- **TweenPositionInternal**(`endPosition: UDim2`, `easingDirection: EasingDirection = Out`, `easingStyle: EasingStyle = Quad`, `time: float = 1`, `override: bool = false`, `callback: Function = nil`) -> `bool`
- **TweenSize**(`endSize: UDim2`, `easingDirection: EasingDirection = Out`, `easingStyle: EasingStyle = Quad`, `time: float = 1`, `override: bool = false`, `callback: Function = nil`) -> `bool`
- **TweenSizeAndPosition**(`endSize: UDim2`, `endPosition: UDim2`, `easingDirection: EasingDirection = Out`, `easingStyle: EasingStyle = Quad`, `time: float = 1`, `override: bool = false`, `callback: Function = nil`) -> `bool`
- **TweenSizeAndPositionInternal**(`endSize: UDim2`, `endPosition: UDim2`, `easingDirection: EasingDirection = Out`, `easingStyle: EasingStyle = Quad`, `time: float = 1`, `override: bool = false`, `callback: Function = nil`) -> `bool`
- **TweenSizeInternal**(`endSize: UDim2`, `easingDirection: EasingDirection = Out`, `easingStyle: EasingStyle = Quad`, `time: float = 1`, `override: bool = false`, `callback: Function = nil`) -> `bool`

## Events

- **DragBegin**(`initialPosition: UDim2`) [Deprecated]
- **DragStopped**(`x: int`, `y: int`) [Deprecated]
- **InputBegan**(`input: InputObject`)
- **InputChanged**(`input: InputObject`)
- **InputEnded**(`input: InputObject`)
- **MouseEnter**(`x: int`, `y: int`)
- **MouseLeave**(`x: int`, `y: int`)
- **MouseMoved**(`x: int`, `y: int`)
- **MouseWheelBackward**(`x: int`, `y: int`)
- **MouseWheelForward**(`x: int`, `y: int`)
- **SelectionGained**()
- **SelectionLost**()
- **TouchLongPress**(`touchPositions: Array`, `state: UserInputState`)
- **TouchPan**(`touchPositions: Array`, `totalTranslation: Vector2`, `velocity: Vector2`, `state: UserInputState`)
- **TouchPinch**(`touchPositions: Array`, `scale: float`, `velocity: float`, `state: UserInputState`)
- **TouchRotate**(`touchPositions: Array`, `rotation: float`, `velocity: float`, `state: UserInputState`)
- **TouchSwipe**(`swipeDirection: SwipeDirection`, `numberOfTouches: int`)
- **TouchTap**(`touchPositions: Array`)
