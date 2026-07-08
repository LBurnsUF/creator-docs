---
title: Chat
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# Chat

Houses the Luau code responsible for running the legacy chat system.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

The **Chat** service houses the Luau code responsible for running the
[legacy chat system](../../../chat/in-experience-text-chat.md#migrate-from-legacy-chat).
Similar to `Class.StarterPlayerScripts`, default objects like
`Class.Script|Scripts` and `Class.ModuleScript|ModuleScripts` are inserted
into the service.

> **Deprecated:** This class is deprecated. Use `Class.TextChatService` instead.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Chat.BubbleChatEnabled` | `bool` |  |
| `Class.Chat.IsAutoMigrated` | `bool` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.Chat.LoadDefaultChat` | `bool` |  {write: NotAccessibleSecurity} |
| `Class.Chat.ModerationMode` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |

## Methods

### `Class.Chat:CanUserChatAsync`

``CanUserChatAsync(userId: `int64`)`` -> `bool`
  [Yields]

### `Class.Chat:CanUsersChatAsync`

``CanUsersChatAsync(userIdFrom: `int64`, userIdTo: `int64`)`` -> `bool`
  [Yields]

### `Class.Chat:Chat`

``Chat(partOrCharacter: `Class.Instance`, message: `string`, color: `Enum.ChatColor`)`` -> `null`

### `Class.Chat:ChatLocal`

``ChatLocal(partOrCharacter: `Class.Instance`, message: `string`, color: `Enum.ChatColor`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.Chat:FilterStringAsync`

``FilterStringAsync(stringToFilter: `string`, playerFrom: `Class.Player`, playerTo: `Class.Player`)`` -> `string`
  [Yields]

### `Class.Chat:FilterStringForBroadcast`

``FilterStringForBroadcast(stringToFilter: `string`, playerFrom: `Class.Player`)`` -> `string`
  [Yields]

### `Class.Chat:FilterStringForPlayerAsync`

``FilterStringForPlayerAsync(stringToFilter: `string`, playerToFilterFor: `Class.Player`)`` -> `string`
  [Yields] [Deprecated]

### `Class.Chat:GetShouldUseLuaChat`

``GetShouldUseLuaChat()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.Chat:InvokeChatCallback`

``InvokeChatCallback(callbackType: `Enum.ChatCallbackType`, callbackArguments: `Tuple`)`` -> `Tuple`

### `Class.Chat:ReconcileCommunicationAccess`

``ReconcileCommunicationAccess()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.Chat:RegisterChatCallback`

``RegisterChatCallback(callbackType: `Enum.ChatCallbackType`, callbackFunction: `Datatype.Function`)`` -> `null`

### `Class.Chat:RequestModerationModeEnabled`

``RequestModerationModeEnabled(enabled: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.Chat:SetBubbleChatSettings`

``SetBubbleChatSettings(settings: `Variant`)`` -> `null`

## Events

### `Class.Chat.BubbleChatSettingsChanged`

Fires with: (settings: `Variant`)

### `Class.Chat.Chatted`

Fires with: (part: `Class.Instance`, message: `string`, color: `Enum.ChatColor`)

### `Class.Chat.PlayerChatAvailabilityStatusChanged`

Fires with: (player: `Class.Player`)

### `Class.Chat.ReconcileCommunicationAccessCompleted`

Fires with: (chatAvailabilityStatus: `string`)

### `Class.Chat.TimeoutChatAttempt`

Fires with: (isPermanentTimeout: `bool`, endTime: `int64`)
