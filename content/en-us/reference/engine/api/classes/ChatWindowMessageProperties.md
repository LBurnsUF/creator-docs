---
title: ChatWindowMessageProperties
type: class
superclass: TextChatMessageProperties
tags: [NotCreatable]
---

# ChatWindowMessageProperties

**Inherits from:** `Class.TextChatMessageProperties` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

Can be used to customize the appearance of text chat messages sent to the
ChatWindow. Inherits from `Class.TextChatMessageProperies`. To create a new
`ChatWindowMessageProperties` instance, use
`Class.ChatWindowConfiguration:DeriveNewMessageProperties()` which will have
the current properties from `Class.ChatWindowConfiguration`.

```lua
local TextChatService = game:GetService("TextChatService")

local ChatWindowConfiguration = TextChatService:FindFirstChildOfClass("ChatWindowConfiguration")

TextChatService.OnChatWindowAdded = function(message: TextChatMessage)
  -- Derive chat message properties
  local properties = ChatWindowConfiguration:DeriveNewMessageProperties()

  -- Change color of message within the chat window
  properties.TextColor3 = Color3.fromRGB(255, 121, 121)

  return properties
end
```

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ChatWindowMessageProperties.FontFace` | `Datatype.Font` |  |
| `Class.ChatWindowMessageProperties.PrefixTextProperties` | `Class.ChatWindowMessageProperties` |  |
| `Class.ChatWindowMessageProperties.TextColor3` | `Datatype.Color3` |  |
| `Class.ChatWindowMessageProperties.TextSize` | `int` |  |
| `Class.ChatWindowMessageProperties.TextStrokeColor3` | `Datatype.Color3` |  |
| `Class.ChatWindowMessageProperties.TextStrokeTransparency` | `double` |  |
