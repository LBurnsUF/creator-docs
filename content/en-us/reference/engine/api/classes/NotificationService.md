---
title: NotificationService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# NotificationService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.NotificationService.IsConnected` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.NotificationService.IsLuaChatEnabled` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.NotificationService.IsLuaGameDetailsEnabled` | `bool` | [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.NotificationService.SelectedTheme` | `string` | [NotReplicated] {security: RobloxScriptSecurity} |

## Methods

### `Class.NotificationService:ActionEnabled`

``ActionEnabled(actionType: `Enum.AppShellActionType`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.NotificationService:ActionTaken`

``ActionTaken(actionType: `Enum.AppShellActionType`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.NotificationService:CancelAllNotification`

``CancelAllNotification(userId: `int64`)`` → `null`
   {security: LocalUserSecurity}

### `Class.NotificationService:CancelNotification`

``CancelNotification(userId: `int64`, alertId: `int`)`` → `null`
   {security: LocalUserSecurity}

### `Class.NotificationService:GetScheduledNotifications`

``GetScheduledNotifications(userId: `int64`)`` → `Array`
  [Yields] {security: LocalUserSecurity}

### `Class.NotificationService:ScheduleNotification`

``ScheduleNotification(userId: `int64`, alertId: `int`, alertMsg: `string`, minutesToFire: `int`)`` → `null`
   {security: LocalUserSecurity}

### `Class.NotificationService:SubscribeToRccEventNamespace`

``SubscribeToRccEventNamespace(eventNamespace: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.NotificationService:SwitchedToAppShellFeature`

``SwitchedToAppShellFeature(appShellFeature: `Enum.AppShellFeature`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.NotificationService.RccConnectionChanged`

Fires with: (connectionName: `string`, connectionState: `Enum.ConnectionState`, rccSequenceNumber: `string`, userIdToNamespaceSequenceNumbers: `Map`)

### `Class.NotificationService.RccEventReceived`

Fires with: (eventData: `Map`, userId: `int64`)

### `Class.NotificationService.Roblox17sConnectionChanged`

Fires with: (connectionName: `string`, connectionState: `Enum.ConnectionState`, namespaceSequenceNumbers: `string`)

### `Class.NotificationService.Roblox17sEventReceived`

Fires with: (eventData: `Map`)

### `Class.NotificationService.RobloxConnectionChanged`

Fires with: (connectionName: `string`, connectionState: `Enum.ConnectionState`, sequenceNumber: `string`, namespaceSequenceNumbers: `string`)

### `Class.NotificationService.RobloxEventReceived`

Fires with: (eventData: `Map`)
