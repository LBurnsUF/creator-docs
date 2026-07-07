---
title: TextBox
type: class
superclass: GuiObject
---

# TextBox

**Inherits from:** `Class.GuiObject` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.TextBox.ClearTextOnFocus` | `bool` |  |
| `Class.TextBox.ContentText` | `string` | [ReadOnly] [NotReplicated] |
| `Class.TextBox.CursorPosition` | `int` |  |
| `Class.TextBox.Font` | `Enum.Font` | [Hidden] [NotReplicated] |
| `Class.TextBox.FontFace` | `Datatype.Font` |  |
| `Class.TextBox.FontSize` | `Enum.FontSize` | [NotReplicated] [Deprecated] |
| `Class.TextBox.LineHeight` | `float` |  |
| `Class.TextBox.LocalizationMatchIdentifier` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.TextBox.LocalizationMatchedSourceText` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.TextBox.ManualFocusRelease` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.TextBox.MaxVisibleGraphemes` | `int` |  |
| `Class.TextBox.MultiLine` | `bool` |  |
| `Class.TextBox.OpenTypeFeatures` | `string` |  |
| `Class.TextBox.OpenTypeFeaturesError` | `string` | [ReadOnly] [NotReplicated] |
| `Class.TextBox.OverlayNativeInput` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.TextBox.PlaceholderColor3` | `Datatype.Color3` |  |
| `Class.TextBox.PlaceholderText` | `string` |  |
| `Class.TextBox.ReturnKeyType` | `Enum.ReturnKeyType` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.TextBox.RichText` | `bool` |  |
| `Class.TextBox.SelectionStart` | `int` |  |
| `Class.TextBox.ShouldEmitReturnEvents` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.TextBox.ShouldEmitTabEvents` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.TextBox.ShouldEmitUpAndDownArrowEvents` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.TextBox.ShowNativeInput` | `bool` |  |
| `Class.TextBox.Text` | `string` |  |
| `Class.TextBox.TextBounds` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] |
| `Class.TextBox.TextColor` | `Datatype.BrickColor` | [Hidden] [NotReplicated] [Deprecated] |
| `Class.TextBox.TextColor3` | `Datatype.Color3` |  |
| `Class.TextBox.TextDirection` | `Enum.TextDirection` |  |
| `Class.TextBox.TextEditable` | `bool` |  |
| `Class.TextBox.TextFits` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.TextBox.TextInputType` | `Enum.TextInputType` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.TextBox.TextScaled` | `bool` |  |
| `Class.TextBox.TextSize` | `float` |  |
| `Class.TextBox.TextStrokeColor3` | `Datatype.Color3` |  |
| `Class.TextBox.TextStrokeTransparency` | `float` |  |
| `Class.TextBox.TextTransparency` | `float` |  |
| `Class.TextBox.TextTruncate` | `Enum.TextTruncate` |  |
| `Class.TextBox.TextWrap` | `bool` | [NotReplicated] [Deprecated] |
| `Class.TextBox.TextWrapped` | `bool` |  |
| `Class.TextBox.TextXAlignment` | `Enum.TextXAlignment` |  |
| `Class.TextBox.TextYAlignment` | `Enum.TextYAlignment` |  |

## Methods

### `Class.TextBox:CaptureFocus`

``CaptureFocus()`` → `null`

### `Class.TextBox:IsFocused`

``IsFocused()`` → `bool`

### `Class.TextBox:ReleaseFocus`

``ReleaseFocus(submitted: `bool`)`` → `null`

### `Class.TextBox:ResetKeyboardMode`

``ResetKeyboardMode()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.TextBox:SetTextFromInput`

``SetTextFromInput(text: `string`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.TextBox.FocusLost`

Fires with: (enterPressed: `bool`, inputThatCausedFocusLoss: `Class.InputObject`)

### `Class.TextBox.Focused`

Fires with: ()

### `Class.TextBox.ReturnPressedFromOnScreenKeyboard`

Fires with: ()
