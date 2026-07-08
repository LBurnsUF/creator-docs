---
title: TextChannel
type: class
superclass: Instance
---

# TextChannel

Represents a text chat channel.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

Represents a text chat channel. Contains `Class.TextSource|TextSources` as
descendants.

To send a chat message to the `Class.TextChannel`, call
`Class.TextChannel:SendAsync()` from a `Class.LocalScript`. The corresponding
`Class.TextSource` of the user with `TextSource.CanSend = true` must be in
that channel.

Messages from different TextChannels can be separated into different tabs in
the chat window using `Class.ChannelTabsConfiguration`.

To learn more, see
[In-Experience Text Chat](../../../chat/in-experience-text-chat.md).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.TextChannel.DirectChatRequester` | `Class.Player` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.TextChannel:AddUserAsync`

``AddUserAsync(userId: `Datatype.User`)`` -> `Tuple`
  [Yields]

### `Class.TextChannel:DisplaySystemMessage`

``DisplaySystemMessage(systemMessage: `string`, metadata: `string`)`` -> `Class.TextChatMessage`

### `Class.TextChannel:SendAsync`

``SendAsync(message: `string`, metadata: `string`)`` -> `Class.TextChatMessage`
  [Yields]

### `Class.TextChannel:SendDictatedSpeechAsync`

``SendDictatedSpeechAsync(message: `string`)`` -> `Class.TextChatMessage`
  [Yields] {security: RobloxScriptSecurity}

### `Class.TextChannel:SendInternalAsync`

``SendInternalAsync(message: `string`, metadata: `string`)`` -> `Class.TextChatMessage`
  [Yields] {security: RobloxScriptSecurity}

### `Class.TextChannel:SendPresetAsync`

``SendPresetAsync(presetId: `string`)`` -> `Class.TextChatMessage`
  [Yields] {security: RobloxScriptSecurity}

### `Class.TextChannel:SetDirectChatRequester`

``SetDirectChatRequester(requester: `Class.Player`)`` -> `null`

## Events

### `Class.TextChannel.MessageReceived`

Fires with: (incomingMessage: `Class.TextChatMessage`)

## Callbacks

### `Class.TextChannel.OnIncomingMessage`

``OnIncomingMessage(message: `Class.TextChatMessage`)`` -> `Tuple`

### `Class.TextChannel.ShouldDeliverCallback`

``ShouldDeliverCallback(message: `Class.TextChatMessage`, textSource: `Class.TextSource`)`` -> `Tuple`
