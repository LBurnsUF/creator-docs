---
title: TextLabel
type: class
superclass: GuiLabel
---

# TextLabel

A 2D user interface element that displays non-interactive text.

**Inherits from:** `Class.GuiLabel` > `Class.GuiObject` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Description

A `Class.TextLabel` renders a rectangle, like a `Class.Frame`, with styled
text. The rectangle can be used to define text boundaries, text scaling
(`Class.TextLabel.TextScaled|TextScaled`), wrapping
(`Class.TextLabel.TextWrapped|TextWrapped`), and alignment
(`Class.TextLabel.TextXAlignment|TextXAlignment` and/or
`Class.TextLabel.TextYAlignment|TextYAlignment`).

This class contains properties that control the display of the text, such as
`Class.TextLabel.Font|Font` and `Class.TextLabel.TextColor3|TextColor3`. To
display only text and hide the background rectangle, set
`Class.TextLabel.BackgroundTransparency|BackgroundTransparency` to `1`.

A `Class.UITextSizeConstraint` object can be used to constrain the size of
text with `Class.TextLabel.TextScaled|TextScaled` enabled. It is recommended
that the size of text is no lower than `9`, otherwise it may not be visible to
many users.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.TextLabel.ContentText` | `string` | [ReadOnly] [NotReplicated] |
| `Class.TextLabel.Font` | `Enum.Font` | [Hidden] [NotReplicated] |
| `Class.TextLabel.FontFace` | `Datatype.Font` |  |
| `Class.TextLabel.FontSize` | `Enum.FontSize` | [NotReplicated] [Deprecated] |
| `Class.TextLabel.LineHeight` | `float` |  |
| `Class.TextLabel.LocalizationMatchIdentifier` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.TextLabel.LocalizationMatchedSourceText` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.TextLabel.LocalizedText` | `string` | [Hidden] [ReadOnly] [NotReplicated] |
| `Class.TextLabel.MaxVisibleGraphemes` | `int` |  |
| `Class.TextLabel.OpenTypeFeatures` | `string` |  |
| `Class.TextLabel.OpenTypeFeaturesError` | `string` | [ReadOnly] [NotReplicated] |
| `Class.TextLabel.RichText` | `bool` |  |
| `Class.TextLabel.Text` | `string` |  |
| `Class.TextLabel.TextBounds` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] |
| `Class.TextLabel.TextColor` | `Datatype.BrickColor` | [Hidden] [NotReplicated] [Deprecated] |
| `Class.TextLabel.TextColor3` | `Datatype.Color3` |  |
| `Class.TextLabel.TextDirection` | `Enum.TextDirection` |  |
| `Class.TextLabel.TextFits` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.TextLabel.TextScaled` | `bool` |  |
| `Class.TextLabel.TextSize` | `float` |  |
| `Class.TextLabel.TextStrokeColor3` | `Datatype.Color3` |  |
| `Class.TextLabel.TextStrokeTransparency` | `float` |  |
| `Class.TextLabel.TextTransparency` | `float` |  |
| `Class.TextLabel.TextTruncate` | `Enum.TextTruncate` |  |
| `Class.TextLabel.TextWrap` | `bool` | [NotReplicated] [Deprecated] |
| `Class.TextLabel.TextWrapped` | `bool` |  |
| `Class.TextLabel.TextXAlignment` | `Enum.TextXAlignment` |  |
| `Class.TextLabel.TextYAlignment` | `Enum.TextYAlignment` |  |

## Methods

### `Class.TextLabel:SetTextFromInput`

``SetTextFromInput(text: `string`)`` -> `null`
   {security: RobloxScriptSecurity}
