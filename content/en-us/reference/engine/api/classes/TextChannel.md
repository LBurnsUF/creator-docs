---
title: TextChannel
type: class
superclass: Instance
---

# TextChannel

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.TextChannel.DirectChatRequester` | `Class.Player` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.TextChannel:AddUserAsync`

``AddUserAsync(userId: `Datatype.User`)`` → `Tuple`
  [Yields]

### `Class.TextChannel:DisplaySystemMessage`

``DisplaySystemMessage(systemMessage: `string`, metadata: `string`)`` → `Class.TextChatMessage`

### `Class.TextChannel:SendAsync`

``SendAsync(message: `string`, metadata: `string`)`` → `Class.TextChatMessage`
  [Yields]

### `Class.TextChannel:SendDictatedSpeechAsync`

``SendDictatedSpeechAsync(message: `string`)`` → `Class.TextChatMessage`
  [Yields] {security: RobloxScriptSecurity}

### `Class.TextChannel:SendInternalAsync`

``SendInternalAsync(message: `string`, metadata: `string`)`` → `Class.TextChatMessage`
  [Yields] {security: RobloxScriptSecurity}

### `Class.TextChannel:SendPresetAsync`

``SendPresetAsync(presetId: `string`)`` → `Class.TextChatMessage`
  [Yields] {security: RobloxScriptSecurity}

### `Class.TextChannel:SetDirectChatRequester`

``SetDirectChatRequester(requester: `Class.Player`)`` → `null`

## Events

### `Class.TextChannel.MessageReceived`

Fires with: (incomingMessage: `Class.TextChatMessage`)

## Callbacks

### `Class.TextChannel.OnIncomingMessage`

``OnIncomingMessage(message: `Class.TextChatMessage`)`` → `Tuple`

### `Class.TextChannel.ShouldDeliverCallback`

``ShouldDeliverCallback(message: `Class.TextChatMessage`, textSource: `Class.TextSource`)`` → `Tuple`
