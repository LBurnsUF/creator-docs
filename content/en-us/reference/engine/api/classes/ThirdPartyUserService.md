---
title: ThirdPartyUserService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ThirdPartyUserService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.ThirdPartyUserService.FriendCommunicationRestrictionStatus` | `Enum.ChatRestrictionStatus` | [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.ThirdPartyUserService.HasActiveUser` | `bool` | [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.ThirdPartyUserService.VoiceChatRestrictionStatus` | `Enum.ChatRestrictionStatus` | [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |

## Methods

### `Class.ThirdPartyUserService:GetUserPlatformName`

``GetUserPlatformName()`` → `string`
   {security: RobloxScriptSecurity}

### `Class.ThirdPartyUserService:GetVoiceChatRestrictionStatus`

``GetVoiceChatRestrictionStatus()`` → `Enum.ChatRestrictionStatus`
   {security: RobloxScriptSecurity}

### `Class.ThirdPartyUserService:HaveActiveUser`

``HaveActiveUser()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.ThirdPartyUserService:IsAccountSwitchingSupported`

``IsAccountSwitchingSupported()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.ThirdPartyUserService:IsChatRestrictionSupported`

``IsChatRestrictionSupported()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.ThirdPartyUserService:IsSingleSignOnSupported`

``IsSingleSignOnSupported()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.ThirdPartyUserService:RegisterActiveUser`

``RegisterActiveUser(gamepadId: `Enum.UserInputType`)`` → `int`
  [Yields] {security: RobloxScriptSecurity}

### `Class.ThirdPartyUserService:ShowAccountPicker`

``ShowAccountPicker()`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.ThirdPartyUserService.ActiveUserSignedOut`

Fires with: (signOutStatus: `int`)
