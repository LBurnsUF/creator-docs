---
title: TextBox
type: class
superclass: GuiObject
---

# TextBox

**Inherits**: GuiObject > GuiBase2d > GuiBase > Instance > Object

## Properties

- **ClearTextOnFocus**: `bool`
- **ContentText**: `string` [ReadOnly] [NotReplicated]
- **CursorPosition**: `int`
- **Font**: `Font` [Hidden] [NotReplicated]
- **FontFace**: `Font`
- **FontSize**: `FontSize` [NotReplicated] [Deprecated]
- **LineHeight**: `float`
- **LocalizationMatchIdentifier**: `string` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **LocalizationMatchedSourceText**: `string` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **ManualFocusRelease**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **MaxVisibleGraphemes**: `int`
- **MultiLine**: `bool`
- **OpenTypeFeatures**: `string`
- **OpenTypeFeaturesError**: `string` [ReadOnly] [NotReplicated]
- **OverlayNativeInput**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **PlaceholderColor3**: `Color3`
- **PlaceholderText**: `string`
- **ReturnKeyType**: `ReturnKeyType` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **RichText**: `bool`
- **SelectionStart**: `int`
- **ShouldEmitReturnEvents**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **ShouldEmitTabEvents**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **ShouldEmitUpAndDownArrowEvents**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **ShowNativeInput**: `bool`
- **Text**: `string`
- **TextBounds**: `Vector2` [ReadOnly] [NotReplicated]
- **TextColor**: `BrickColor` [Hidden] [NotReplicated] [Deprecated]
- **TextColor3**: `Color3`
- **TextDirection**: `TextDirection`
- **TextEditable**: `bool`
- **TextFits**: `bool` [ReadOnly] [NotReplicated]
- **TextInputType**: `TextInputType` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **TextScaled**: `bool`
- **TextSize**: `float`
- **TextStrokeColor3**: `Color3`
- **TextStrokeTransparency**: `float`
- **TextTransparency**: `float`
- **TextTruncate**: `TextTruncate`
- **TextWrap**: `bool` [NotReplicated] [Deprecated]
- **TextWrapped**: `bool`
- **TextXAlignment**: `TextXAlignment`
- **TextYAlignment**: `TextYAlignment`

## Methods

- **CaptureFocus**() -> `null`
- **IsFocused**() -> `bool`
- **ReleaseFocus**(`submitted: bool = false`) -> `null`
- **ResetKeyboardMode**() -> `null`
- **SetTextFromInput**(`text: string`) -> `null`

## Events

- **FocusLost**(`enterPressed: bool`, `inputThatCausedFocusLoss: InputObject`)
- **Focused**()
- **ReturnPressedFromOnScreenKeyboard**()
