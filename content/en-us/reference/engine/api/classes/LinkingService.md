---
title: LinkingService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# LinkingService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.LinkingService:DetectUrl`

``DetectUrl(url: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.LinkingService:GetAndClearLastPendingUrl`

``GetAndClearLastPendingUrl()`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.LinkingService:GetLastLuaUrl`

``GetLastLuaUrl()`` → `string?`
   {security: RobloxScriptSecurity}

### `Class.LinkingService:IsUrlRegistered`

``IsUrlRegistered(url: `string`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.LinkingService:OpenUrl`

``OpenUrl(url: `string`)`` → `bool`
  [Yields] {security: RobloxScriptSecurity}

### `Class.LinkingService:RegisterLuaUrl`

``RegisterLuaUrl(url: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.LinkingService:StartLuaUrlDelivery`

``StartLuaUrlDelivery()`` → `Dictionary?`
   {security: RobloxScriptSecurity}

### `Class.LinkingService:StopLuaUrlDelivery`

``StopLuaUrlDelivery()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.LinkingService:SupportsSwitchToSettingsApp`

``SupportsSwitchToSettingsApp()`` → `bool`
  [Yields] {security: RobloxScriptSecurity}

### `Class.LinkingService:SwitchToSettingsApp`

``SwitchToSettingsApp(route: `string?`)`` → `null`
  [Yields] {security: RobloxScriptSecurity}

## Events

### `Class.LinkingService.OnLuaUrl`

Fires with: (url: `string`, matchedUrl: `string`, attributionUrl: `string?`)
