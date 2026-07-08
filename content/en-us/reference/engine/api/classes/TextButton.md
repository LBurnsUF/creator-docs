---
title: TextButton
type: class
superclass: GuiButton
---

# TextButton

A 2D user interface element that displays interactive text.

**Inherits from:** `Class.GuiButton` > `Class.GuiObject` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Description

A `Class.TextButton` behaves similarly to `Class.TextLabel` in regards to
rendering, with the additional behaviors of a `Class.GuiButton`.

You can disable text rendering by setting
`Class.TextButton.TextTransparency|TextTransparency` to `1`. This will result
in a plain rectangle that can be used as a button.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.TextButton.ContentText` | `string` | [ReadOnly] [NotReplicated] |
| `Class.TextButton.Font` | `Enum.Font` | [Hidden] [NotReplicated] |
| `Class.TextButton.FontFace` | `Datatype.Font` |  |
| `Class.TextButton.FontSize` | `Enum.FontSize` | [NotReplicated] [Deprecated] |
| `Class.TextButton.LineHeight` | `float` |  |
| `Class.TextButton.LocalizationMatchIdentifier` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.TextButton.LocalizationMatchedSourceText` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.TextButton.LocalizedText` | `string` | [Hidden] [ReadOnly] [NotReplicated] |
| `Class.TextButton.MaxVisibleGraphemes` | `int` |  |
| `Class.TextButton.OpenTypeFeatures` | `string` |  |
| `Class.TextButton.OpenTypeFeaturesError` | `string` | [ReadOnly] [NotReplicated] |
| `Class.TextButton.RichText` | `bool` |  |
| `Class.TextButton.Text` | `string` |  |
| `Class.TextButton.TextBounds` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] |
| `Class.TextButton.TextColor` | `Datatype.BrickColor` | [Hidden] [NotReplicated] [Deprecated] |
| `Class.TextButton.TextColor3` | `Datatype.Color3` |  |
| `Class.TextButton.TextDirection` | `Enum.TextDirection` |  |
| `Class.TextButton.TextFits` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.TextButton.TextScaled` | `bool` |  |
| `Class.TextButton.TextSize` | `float` |  |
| `Class.TextButton.TextStrokeColor3` | `Datatype.Color3` |  |
| `Class.TextButton.TextStrokeTransparency` | `float` |  |
| `Class.TextButton.TextTransparency` | `float` |  |
| `Class.TextButton.TextTruncate` | `Enum.TextTruncate` |  |
| `Class.TextButton.TextWrap` | `bool` | [NotReplicated] [Deprecated] |
| `Class.TextButton.TextWrapped` | `bool` |  |
| `Class.TextButton.TextXAlignment` | `Enum.TextXAlignment` |  |
| `Class.TextButton.TextYAlignment` | `Enum.TextYAlignment` |  |

## Methods

### `Class.TextButton:SetTextFromInput`

``SetTextFromInput(text: `string`)`` -> `null`
   {security: RobloxScriptSecurity}
