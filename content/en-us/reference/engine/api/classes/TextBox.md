---
title: TextBox
type: class
superclass: GuiObject
---

# TextBox

A 2D user interface element that displays player-editable text.

**Inherits from:** `Class.GuiObject` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Description

A `TextBox` allows the player to provide text input. It behaves similarly to a
`Class.TextButton`, except that a single `TextBox` can be put in focus by
clicking, tapping, or gamepad selection. While in focus, the player can use a
keyboard to change the `Class.TextBox.Text|Text` property.

- If there is no text, the `Class.TextBox.PlaceholderText|PlaceholderText`
  will be visible. This is useful prompting players of the kind or format of
  data they should input.
- By default, the `Class.TextBox.ClearTextOnFocus|ClearTextOnFocus` property
  is enabled and ensures there is no existing text when a `TextBox` is
  focused. This may not be desirable for text that should be editable by the
  player.
- The `Class.TextBox.MultiLine|MultiLine` property allows players to enter
  multiple lines of text with newline characters (`\n`).

#### Focus State

It is possible to detect and change the focus state of a `TextBox`:

- You can use `Class.TextBox:CaptureFocus()|CaptureFocus` when a dialogue
  appears so that the player doesn't have to click on a `TextBox` when it
  becomes available; you can use `Class.ContextActionService:BindAction()` to
  bind a certain key to focus a `TextBox` using this function. When a
  `TextBox` comes into focus, the `Class.TextBox.Focused|Focused` event fires.
- You can detect if a certain `TextBox` is in focus by using
  `Class.TextBox:IsFocused()|IsFocused`. Alternatively,
  `Class.UserInputService:GetFocusedTextBox()` can be used to check if any
  `TextBox` is in focus.
- When the player is done inputting text, the
  `Class.TextBox.FocusLost|FocusLost` event fires, indicating if the player
  pressed <kbd>Enter</kbd> to submit text along with the `Class.InputObject`
  that caused the loss of focus. When using on-screen keyboards on mobile and
  console,
  `Class.TextBox.ReturnPressedFromOnScreenKeyboard|ReturnPressedFromOnScreenKeyboard`
  may also fire.
- If some more important matter comes up during gameplay, you can
  `Class.TextBox:ReleaseFocus()|ReleaseFocus` of the `TextBox` so that a
  player's keyboard input returns to your game.

#### Text Editing

A `TextBox` supports text selection through its
`Class.TextBox.CursorPosition|CursorPosition` and
`Class.TextBox.SelectionStart|SelectionStart` properties. Using
`Class.Object:GetPropertyChangedSignal()|GetPropertyChangedSignal`, you can
detect when a selection changes. Additionally, it is possible for players to
copy and paste text within a TextBox, enabling basic clipboard support.

**Text Filtering Notice** Games that facilitate player-to-player communication
using text, such as custom chat or nametags, must properly filter such text
using `Class.TextService:FilterStringAsync()` or
`Class.Chat:FilterStringAsync()`. If this is not properly done, your game may
receive moderation action.

## Properties

| Property | Type | Description |
|----------|------|-------------|
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

``CaptureFocus()`` -> `null`

### `Class.TextBox:IsFocused`

``IsFocused()`` -> `bool`

### `Class.TextBox:ReleaseFocus`

``ReleaseFocus(submitted: `bool`)`` -> `null`

### `Class.TextBox:ResetKeyboardMode`

``ResetKeyboardMode()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.TextBox:SetTextFromInput`

``SetTextFromInput(text: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.TextBox.FocusLost`

Fires with: (enterPressed: `bool`, inputThatCausedFocusLoss: `Class.InputObject`)

### `Class.TextBox.Focused`

Fires with: ()

### `Class.TextBox.ReturnPressedFromOnScreenKeyboard`

Fires with: ()
