---
title: AccountService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# AccountService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.AccountService:DeviceAccessTokenAvailable`

``DeviceAccessTokenAvailable()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.AccountService:DeviceIntegrityAvailable`

``DeviceIntegrityAvailable()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.AccountService:GetCredentialsHeaders`

``GetCredentialsHeaders()`` → `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AccountService:GetDeviceAccessToken`

``GetDeviceAccessToken()`` → `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AccountService:GetDeviceIntegrityToken`

``GetDeviceIntegrityToken(data: `string`)`` → `string`
   {security: RobloxScriptSecurity}

### `Class.AccountService:GetDeviceIntegrityTokenYield`

``GetDeviceIntegrityTokenYield(data: `string`)`` → `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AccountService:MagicLogin`

``MagicLogin(data: `string`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.AccountService.MagicLoginEvent`

Fires with: (data: `string`)
