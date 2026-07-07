---
title: ScrollingFrame
type: class
superclass: GuiObject
---

# ScrollingFrame

**Inherits**: GuiObject > GuiBase2d > GuiBase > Instance > Object

## Properties

- **AbsoluteCanvasSize**: `Vector2` [ReadOnly] [NotReplicated]
- **AbsoluteWindowSize**: `Vector2` [ReadOnly] [NotReplicated]
- **AutomaticCanvasSize**: `AutomaticSize`
- **BottomImage**: `ContentId`
- **BottomImageContent**: `Content`
- **CanvasPosition**: `Vector2`
- **CanvasSize**: `UDim2`
- **DraggingScrollBar**: `DraggingScrollBar` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **ElasticBehavior**: `ElasticBehavior`
- **HorizontalBarRect**: `Rect` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **HorizontalScrollBarInset**: `ScrollBarInset`
- **MaxCanvasPosition**: `Vector2` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **MidImage**: `ContentId`
- **MidImageContent**: `Content`
- **ScrollBarImageColor3**: `Color3`
- **ScrollBarImageTransparency**: `float`
- **ScrollBarThickness**: `int`
- **ScrollRate**: `float` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **ScrollVelocity**: `Vector2` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **ScrollingDirection**: `ScrollingDirection`
- **ScrollingEnabled**: `bool`
- **SmoothScroll**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **TopImage**: `ContentId`
- **TopImageContent**: `Content`
- **VerticalBarRect**: `Rect` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **VerticalScrollBarInset**: `ScrollBarInset`
- **VerticalScrollBarPosition**: `VerticalScrollBarPosition`

## Methods

- **ClearInertialScrolling**() -> `null`
- **GetSampledInertialVelocity**() -> `Vector2`
- **GetScrollVelocity**() -> `Vector2`
- **ResetScrollVelocity**() -> `null`
- **ScrollToTop**() -> `null`
