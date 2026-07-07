---
title: TextChannel
type: class
superclass: Instance
---

# TextChannel

**Inherits**: Instance > Object

## Properties

- **DirectChatRequester**: `Player` [ReadOnly] [NotReplicated]

## Methods

- **AddUserAsync**(`userId: User`) -> `Tuple` [Yields]
- **DisplaySystemMessage**(`systemMessage: string`, `metadata: string = `) -> `TextChatMessage`
- **SendAsync**(`message: string`, `metadata: string = `) -> `TextChatMessage` [Yields]
- **SendDictatedSpeechAsync**(`message: string`) -> `TextChatMessage` [Yields]
- **SendInternalAsync**(`message: string`, `metadata: string = `) -> `TextChatMessage` [Yields]
- **SendPresetAsync**(`presetId: string`) -> `TextChatMessage` [Yields]
- **SetDirectChatRequester**(`requester: Player`) -> `null`

## Events

- **MessageReceived**(`incomingMessage: TextChatMessage`)

## Callbacks

- **OnIncomingMessage**(`message: TextChatMessage`) -> `Tuple`
- **ShouldDeliverCallback**(`message: TextChatMessage`, `textSource: TextSource`) -> `Tuple`
