---
title: ChatWindowConfiguration
type: class
superclass: TextChatConfigurations
tags: [NotCreatable]
---

# ChatWindowConfiguration

Configures properties of the default chat window.

**Inherits from:** `Class.TextChatConfigurations` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

Configures properties of the default text chat window. It is parented to
`Class.TextChatService`.

#### Chat UI composition

The default chat UI is composed of two separate elements: the **chat window**
(message list) configured by this object, and the **chat input bar**
configured by `Class.ChatInputBarConfiguration`. Each element reports its own
`AbsoluteSize` and `AbsolutePosition` independently. To determine the total
screen bounds of the entire chat UI, combine values from both configurations
by computing the union of the two rectangles.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ChatWindowConfiguration.AbsolutePosition` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] |
| `Class.ChatWindowConfiguration.AbsolutePositionWrite` | `Datatype.Vector2` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.ChatWindowConfiguration.AbsoluteSize` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] |
| `Class.ChatWindowConfiguration.AbsoluteSizeWrite` | `Datatype.Vector2` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.ChatWindowConfiguration.BackgroundColor3` | `Datatype.Color3` |  |
| `Class.ChatWindowConfiguration.BackgroundTransparency` | `double` |  |
| `Class.ChatWindowConfiguration.Enabled` | `bool` |  |
| `Class.ChatWindowConfiguration.FontFace` | `Datatype.Font` |  |
| `Class.ChatWindowConfiguration.HeightScale` | `float` |  |
| `Class.ChatWindowConfiguration.HorizontalAlignment` | `Enum.HorizontalAlignment` |  |
| `Class.ChatWindowConfiguration.TextColor3` | `Datatype.Color3` |  |
| `Class.ChatWindowConfiguration.TextSize` | `int64` |  |
| `Class.ChatWindowConfiguration.TextStrokeColor3` | `Datatype.Color3` |  |
| `Class.ChatWindowConfiguration.TextStrokeTransparency` | `double` |  |
| `Class.ChatWindowConfiguration.VerticalAlignment` | `Enum.VerticalAlignment` |  |
| `Class.ChatWindowConfiguration.WidthScale` | `float` |  |

## Methods

### `Class.ChatWindowConfiguration:DeriveNewMessageProperties`

``DeriveNewMessageProperties()`` -> `Class.ChatWindowMessageProperties`
