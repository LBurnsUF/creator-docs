---
title: GuiBase2d
type: class
superclass: GuiBase
tags: [NotCreatable, NotBrowsable]
---

# GuiBase2d

**Inherits**: GuiBase > Instance > Object

**Tags**: NotCreatable, NotBrowsable

## Properties

- **AbsolutePosition**: `Vector2` [ReadOnly] [NotReplicated]
- **AbsoluteRotation**: `float` [ReadOnly] [NotReplicated]
- **AbsoluteSize**: `Vector2` [ReadOnly] [NotReplicated]
- **AutoLocalize**: `bool`
- **ClippedRect**: `Rect` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **IsNotOccluded**: `bool` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Localize**: `bool` [Hidden] [NotReplicated] [Deprecated]
- **RawRect2D**: `Rect` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **RootLocalizationTable**: `LocalizationTable`
- **SelectionBehaviorDown**: `SelectionBehavior`
- **SelectionBehaviorLeft**: `SelectionBehavior`
- **SelectionBehaviorRight**: `SelectionBehavior`
- **SelectionBehaviorUp**: `SelectionBehavior`
- **SelectionGroup**: `bool`
- **TotalGroupScale**: `float` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Events

- **SelectionChanged**(`amISelected: bool`, `previousSelection: GuiObject`, `newSelection: GuiObject`)
