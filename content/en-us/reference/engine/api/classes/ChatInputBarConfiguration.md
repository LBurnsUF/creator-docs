---
title: ChatInputBarConfiguration
type: class
superclass: TextChatConfigurations
tags: [NotCreatable]
---

# ChatInputBarConfiguration

Configures properties of the default chat input bar.

**Inherits from:** `Class.TextChatConfigurations` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

Configures properties of the default text chat input bar. It is parented to
`Class.TextChatService`.

#### Chat UI composition

The default chat UI is composed of two separate elements: the **chat window**
(message list) configured by `Class.ChatWindowConfiguration`, and the **chat
input bar** configured by this object. Each element reports its own
`AbsoluteSize` and `AbsolutePosition` independently. To determine the total
screen bounds of the entire chat UI, combine values from both configurations
by computing the union of the two rectangles.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ChatInputBarConfiguration.AbsolutePosition` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] |
| `Class.ChatInputBarConfiguration.AbsolutePositionWrite` | `Datatype.Vector2` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.ChatInputBarConfiguration.AbsoluteSize` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] |
| `Class.ChatInputBarConfiguration.AbsoluteSizeWrite` | `Datatype.Vector2` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.ChatInputBarConfiguration.AutocompleteEnabled` | `bool` |  |
| `Class.ChatInputBarConfiguration.BackgroundColor3` | `Datatype.Color3` |  |
| `Class.ChatInputBarConfiguration.BackgroundTransparency` | `double` |  |
| `Class.ChatInputBarConfiguration.Enabled` | `bool` |  |
| `Class.ChatInputBarConfiguration.FontFace` | `Datatype.Font` |  |
| `Class.ChatInputBarConfiguration.IsFocused` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.ChatInputBarConfiguration.IsFocusedWrite` | `bool` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.ChatInputBarConfiguration.KeyboardKeyCode` | `Enum.KeyCode` |  |
| `Class.ChatInputBarConfiguration.PlaceholderColor3` | `Datatype.Color3` |  |
| `Class.ChatInputBarConfiguration.TargetTextChannel` | `Class.TextChannel` |  |
| `Class.ChatInputBarConfiguration.TextBox` | `Class.TextBox` |  |
| `Class.ChatInputBarConfiguration.TextColor3` | `Datatype.Color3` |  |
| `Class.ChatInputBarConfiguration.TextSize` | `int64` |  |
| `Class.ChatInputBarConfiguration.TextStrokeColor3` | `Datatype.Color3` |  |
| `Class.ChatInputBarConfiguration.TextStrokeTransparency` | `double` |  |
