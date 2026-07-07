---
title: TextChatService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# TextChatService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.TextChatService.ChatTranslationEnabled` | `bool` | [NotReplicated] {write: RobloxScriptSecurity} |
| `Class.TextChatService.ChatTranslationFTUXShown` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.TextChatService.ChatTranslationToggleEnabled` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.TextChatService.ChatVersion` | `Enum.ChatVersion` |  {write: RobloxScriptSecurity} |
| `Class.TextChatService.CreateDefaultCommands` | `bool` |  {write: PluginSecurity} |
| `Class.TextChatService.CreateDefaultTextChannels` | `bool` |  {write: PluginSecurity} |
| `Class.TextChatService.EnableProtectedChat` | `Enum.RolloutState` |  {security: RobloxScriptSecurity} |
| `Class.TextChatService.HasSeenDeprecationDialog` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.TextChatService.IsLegacyChatDisabled` | `bool` | [Hidden] {security: RobloxScriptSecurity} |

## Methods

### `Class.TextChatService:CanUserChatAsync`

``CanUserChatAsync(userId: `Datatype.User`)`` → `bool`
  [Yields]

### `Class.TextChatService:CanUsersChatAsync`

``CanUsersChatAsync(userIdFrom: `Datatype.User`, userIdTo: `Datatype.User`)`` → `bool`
  [Yields]

### `Class.TextChatService:CanUsersDirectChatAsync`

``CanUsersDirectChatAsync(requesterUserId: `Datatype.User`, userIds: `Array`)`` → `Array`
  [Yields]

### `Class.TextChatService:CanUsersWhisperAsync`

``CanUsersWhisperAsync(fromUserId: `Datatype.User`, toUserId: `Datatype.User`)`` → `bool`
  [Yields] {security: RobloxScriptSecurity}

### `Class.TextChatService:DisplayBubble`

``DisplayBubble(partOrCharacter: `Class.Instance`, message: `string`)`` → `null`

### `Class.TextChatService:GetChatGroupsAsync`

``GetChatGroupsAsync(players: `Datatype.Instances`)`` → `Array`
  [Yields]

### `Class.TextChatService:GetChatableUserCountAsync`

``GetChatableUserCountAsync(userId: `Datatype.User`, context: `string`)`` → `int`
  [Yields] {security: RobloxScriptSecurity}

### `Class.TextChatService:GetPresetsAsync`

``GetPresetsAsync()`` → `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.TextChatService:GetTextChannelWindows`

``GetTextChannelWindows()`` → `Array`
   {security: RobloxScriptSecurity}

### `Class.TextChatService:HasAllocatedUniverseChatContext`

``HasAllocatedUniverseChatContext(context: `string`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.TextChatService:OnUserChatSettingUpdateAsync`

``OnUserChatSettingUpdateAsync(featureName: `string`, featureValue: `string`)`` → `bool`
  [Yields] {security: RobloxScriptSecurity}

### `Class.TextChatService:SendDictatedSpeechUniverseChatAsync`

``SendDictatedSpeechUniverseChatAsync(text: `string`)`` → `Class.TextChatMessage`
  [Yields] {security: RobloxScriptSecurity}

### `Class.TextChatService:SendEnableChatButtonClicked`

``SendEnableChatButtonClicked()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.TextChatService:SendEnableChatButtonShown`

``SendEnableChatButtonShown()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.TextChatService:SendExpChatLoadSuccess`

``SendExpChatLoadSuccess(loadingLatency: `int`, extras: `Dictionary?`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.TextChatService:SendExpChatMessageClientRendered`

``SendExpChatMessageClientRendered(textChatMessage: `Class.TextChatMessage`, messageRenderedSurface: `string`, selectedChannelTab: `int64`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.TextChatService:SendExpChatWindowScroll`

``SendExpChatWindowScroll()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.TextChatService:SendExpChatWindowStatusChange`

``SendExpChatWindowStatusChange(timeClosed: `int`, timeOpen: `int`, timeBackgroundIdle: `int`, timeTextIdle: `int`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.TextChatService:SendUniverseChatMessageAsync`

``SendUniverseChatMessageAsync(text: `string`, metadata: `string`)`` → `Class.TextChatMessage`
  [Yields] {security: RobloxScriptSecurity}

### `Class.TextChatService:SendUniverseChatPresetAsync`

``SendUniverseChatPresetAsync(presetId: `string`)`` → `Class.TextChatMessage`
  [Yields] {security: RobloxScriptSecurity}

### `Class.TextChatService:setModerationModeEnabled`

``setModerationModeEnabled(userId: `int64`, enabled: `bool`)`` → `bool`
   {security: RobloxScriptSecurity}

## Events

### `Class.TextChatService.BubbleDisplayed`

Fires with: (partOrCharacter: `Class.Instance`, textChatMessage: `Class.TextChatMessage`)

### `Class.TextChatService.ChatActionReceived`

Fires with: (chatActionMessage: `Class.TextChatMessage`)

### `Class.TextChatService.ExpChatFeatureValueChanged`

Fires with: (userId: `int64`, featureName: `string`, featureValue: `string`)

### `Class.TextChatService.MessageReceived`

Fires with: (textChatMessage: `Class.TextChatMessage`)

### `Class.TextChatService.OnIncomingMessageEvent`

Fires with: (textChatMessage: `Class.TextChatMessage`)

### `Class.TextChatService.SendingMessage`

Fires with: (textChatMessage: `Class.TextChatMessage`)

### `Class.TextChatService.SendingUniverseChatMessage`

Fires with: (textChatMessage: `Class.TextChatMessage`)

### `Class.TextChatService.TextChannelWindowAdded`

Fires with: (textChannelWindow: `Class.TextChannelWindow`)

### `Class.TextChatService.TextChannelWindowRemoved`

Fires with: (textChannelWindow: `Class.TextChannelWindow`)

### `Class.TextChatService.UniverseChatChannelAllocated`

Fires with: (context: `string`)

### `Class.TextChatService.UniverseChatMessageReceived`

Fires with: (textChatMessage: `Class.TextChatMessage`)

### `Class.TextChatService.UserMessageIntentSent`

Fires with: (userIntentMessage: `Class.TextChatMessage`)

## Callbacks

### `Class.TextChatService.OnBubbleAdded`

``OnBubbleAdded(message: `Class.TextChatMessage`, adornee: `Class.Instance`)`` → `Tuple`

### `Class.TextChatService.OnChatWindowAdded`

``OnChatWindowAdded(message: `Class.TextChatMessage`)`` → `Tuple`

### `Class.TextChatService.OnIncomingMessage`

``OnIncomingMessage(message: `Class.TextChatMessage`)`` → `Tuple`
