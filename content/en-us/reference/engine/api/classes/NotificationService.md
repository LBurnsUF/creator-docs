---
title: NotificationService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# NotificationService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **IsConnected**: `bool` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **IsLuaChatEnabled**: `bool` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **IsLuaGameDetailsEnabled**: `bool` [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **SelectedTheme**: `string` [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **ActionEnabled**(`actionType: AppShellActionType`) -> `null`
- **ActionTaken**(`actionType: AppShellActionType`) -> `null`
- **CancelAllNotification**(`userId: int64`) -> `null`
- **CancelNotification**(`userId: int64`, `alertId: int`) -> `null`
- **GetScheduledNotifications**(`userId: int64`) -> `Array` [Yields]
- **ScheduleNotification**(`userId: int64`, `alertId: int`, `alertMsg: string`, `minutesToFire: int`) -> `null`
- **SubscribeToRccEventNamespace**(`eventNamespace: string`) -> `null`
- **SwitchedToAppShellFeature**(`appShellFeature: AppShellFeature`) -> `null`

## Events

- **RccConnectionChanged**(`connectionName: string`, `connectionState: ConnectionState`, `rccSequenceNumber: string`, `userIdToNamespaceSequenceNumbers: Map`)
- **RccEventReceived**(`eventData: Map`, `userId: int64`)
- **Roblox17sConnectionChanged**(`connectionName: string`, `connectionState: ConnectionState`, `namespaceSequenceNumbers: string`)
- **Roblox17sEventReceived**(`eventData: Map`)
- **RobloxConnectionChanged**(`connectionName: string`, `connectionState: ConnectionState`, `sequenceNumber: string`, `namespaceSequenceNumbers: string`)
- **RobloxEventReceived**(`eventData: Map`)
