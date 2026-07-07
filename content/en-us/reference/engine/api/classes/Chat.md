---
title: Chat
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# Chat

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **BubbleChatEnabled**: `bool`
- **IsAutoMigrated**: `bool` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **LoadDefaultChat**: `bool` (Security: Read=None, Write=NotAccessibleSecurity)
- **ModerationMode**: `string` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **CanUserChatAsync**(`userId: int64`) -> `bool` [Yields]
- **CanUsersChatAsync**(`userIdFrom: int64`, `userIdTo: int64`) -> `bool` [Yields]
- **Chat**(`partOrCharacter: Instance`, `message: string`, `color: ChatColor = Blue`) -> `null`
- **ChatLocal**(`partOrCharacter: Instance`, `message: string`, `color: ChatColor = Blue`) -> `null`
- **FilterStringAsync**(`stringToFilter: string`, `playerFrom: Player`, `playerTo: Player`) -> `string` [Yields]
- **FilterStringForBroadcast**(`stringToFilter: string`, `playerFrom: Player`) -> `string` [Yields]
- **FilterStringForPlayerAsync**(`stringToFilter: string`, `playerToFilterFor: Player`) -> `string` [Yields] [Deprecated]
- **GetShouldUseLuaChat**() -> `bool`
- **InvokeChatCallback**(`callbackType: ChatCallbackType`, `callbackArguments: Tuple`) -> `Tuple`
- **ReconcileCommunicationAccess**() -> `null`
- **RegisterChatCallback**(`callbackType: ChatCallbackType`, `callbackFunction: Function`) -> `null`
- **RequestModerationModeEnabled**(`enabled: bool`) -> `null`
- **SetBubbleChatSettings**(`settings: Variant`) -> `null`

## Events

- **BubbleChatSettingsChanged**(`settings: Variant`)
- **Chatted**(`part: Instance`, `message: string`, `color: ChatColor`)
- **PlayerChatAvailabilityStatusChanged**(`player: Player`)
- **ReconcileCommunicationAccessCompleted**(`chatAvailabilityStatus: string`)
- **TimeoutChatAttempt**(`isPermanentTimeout: bool`, `endTime: int64`)
