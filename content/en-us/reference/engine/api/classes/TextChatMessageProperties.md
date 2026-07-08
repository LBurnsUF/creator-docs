---
title: TextChatMessageProperties
type: class
superclass: Instance
---

# TextChatMessageProperties

Overrides `Class.TextChatMessage` properties when returned by callbacks
defined in `Class.TextChatService.OnIncomingMessage` or
`Class.TextChannel.OnIncomingMessage`.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

Overrides `Class.TextChatMessage` properties like
`Class.TextChatMessage.ChatWindowMessageProperties|ChatWindowMessageProperties`
and
`Class.TextChatMessage.BubbleChatMessageProperties|BubbleChatMessageProperties`
when returned by callbacks defined in
`Class.TextChatService.OnIncomingMessage` or
`Class.TextChannel.OnIncomingMessage`. These properties are useful for
customizing the appearance of a message with
[rich text](../../../ui/rich-text.md) tags.

For sample code, see
[Assign chat tags](../../../chat/examples/group-chat-tags.md).

If you return empty strings for any of these properties,
`Class.TextChatService` ignores them and **doesn't** override the original
values.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.TextChatMessageProperties.PrefixText` | `string` |  |
| `Class.TextChatMessageProperties.Text` | `string` |  |
| `Class.TextChatMessageProperties.Translation` | `string` |  |
