---
title: TextChatService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# TextChatService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **ChatTranslationEnabled**: `bool` [NotReplicated] (Security: Read=None, Write=RobloxScriptSecurity)
- **ChatTranslationFTUXShown**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **ChatTranslationToggleEnabled**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **ChatVersion**: `ChatVersion` (Security: Read=None, Write=RobloxScriptSecurity)
- **CreateDefaultCommands**: `bool` (Security: Read=None, Write=PluginSecurity)
- **CreateDefaultTextChannels**: `bool` (Security: Read=None, Write=PluginSecurity)
- **EnableProtectedChat**: `RolloutState` (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **HasSeenDeprecationDialog**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **IsLegacyChatDisabled**: `bool` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **CanUserChatAsync**(`userId: User`) -> `bool` [Yields]
- **CanUsersChatAsync**(`userIdFrom: User`, `userIdTo: User`) -> `bool` [Yields]
- **CanUsersDirectChatAsync**(`requesterUserId: User`, `userIds: Array`) -> `Array` [Yields]
- **CanUsersWhisperAsync**(`fromUserId: User`, `toUserId: User`) -> `bool` [Yields]
- **DisplayBubble**(`partOrCharacter: Instance`, `message: string`) -> `null`
- **GetChatGroupsAsync**(`players: Instances`) -> `Array` [Yields]
- **GetChatableUserCountAsync**(`userId: User`, `context: string`) -> `int` [Yields]
- **GetPresetsAsync**() -> `Dictionary` [Yields]
- **GetTextChannelWindows**() -> `Array`
- **HasAllocatedUniverseChatContext**(`context: string`) -> `bool`
- **OnUserChatSettingUpdateAsync**(`featureName: string`, `featureValue: string`) -> `bool` [Yields]
- **SendDictatedSpeechUniverseChatAsync**(`text: string`) -> `TextChatMessage` [Yields]
- **SendEnableChatButtonClicked**() -> `null`
- **SendEnableChatButtonShown**() -> `null`
- **SendExpChatLoadSuccess**(`loadingLatency: int`, `extras: Dictionary?`) -> `null`
- **SendExpChatMessageClientRendered**(`textChatMessage: TextChatMessage`, `messageRenderedSurface: string = unknown`, `selectedChannelTab: int64 = -1`) -> `null`
- **SendExpChatWindowScroll**() -> `null`
- **SendExpChatWindowStatusChange**(`timeClosed: int`, `timeOpen: int`, `timeBackgroundIdle: int`, `timeTextIdle: int`) -> `null`
- **SendUniverseChatMessageAsync**(`text: string`, `metadata: string`) -> `TextChatMessage` [Yields]
- **SendUniverseChatPresetAsync**(`presetId: string`) -> `TextChatMessage` [Yields]
- **setModerationModeEnabled**(`userId: int64`, `enabled: bool`) -> `bool`

## Events

- **BubbleDisplayed**(`partOrCharacter: Instance`, `textChatMessage: TextChatMessage`)
- **ChatActionReceived**(`chatActionMessage: TextChatMessage`)
- **ExpChatFeatureValueChanged**(`userId: int64`, `featureName: string`, `featureValue: string`)
- **MessageReceived**(`textChatMessage: TextChatMessage`)
- **OnIncomingMessageEvent**(`textChatMessage: TextChatMessage`)
- **SendingMessage**(`textChatMessage: TextChatMessage`)
- **SendingUniverseChatMessage**(`textChatMessage: TextChatMessage`)
- **TextChannelWindowAdded**(`textChannelWindow: TextChannelWindow`)
- **TextChannelWindowRemoved**(`textChannelWindow: TextChannelWindow`)
- **UniverseChatChannelAllocated**(`context: string`)
- **UniverseChatMessageReceived**(`textChatMessage: TextChatMessage`)
- **UserMessageIntentSent**(`userIntentMessage: TextChatMessage`)

## Callbacks

- **OnBubbleAdded**(`message: TextChatMessage`, `adornee: Instance`) -> `Tuple`
- **OnChatWindowAdded**(`message: TextChatMessage`) -> `Tuple`
- **OnIncomingMessage**(`message: TextChatMessage`) -> `Tuple`
