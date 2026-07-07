---
title: AvatarChatService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# AvatarChatService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.AvatarChatService.ClientFeatures` | `int` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.AvatarChatService.ClientFeaturesInitialized` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.AvatarChatService.ServerFeatures` | `int` | [Hidden] {read: RobloxScriptSecurity, write: RobloxSecurity} |

## Methods

### `Class.AvatarChatService:DebugCounterGet`

``DebugCounterGet(label: `string`, playerId: `int64`)`` → `int64`
   {security: RobloxScriptSecurity}

### `Class.AvatarChatService:EnableVoice`

``EnableVoice()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.AvatarChatService:GetClientFeaturesAsync`

``GetClientFeaturesAsync()`` → `int`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AvatarChatService:GetServerFeaturesAsync`

``GetServerFeaturesAsync()`` → `int`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AvatarChatService:IsEnabled`

``IsEnabled(mask: `int`, feature: `Enum.AvatarChatServiceFeature`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.AvatarChatService:IsPlaceEnabled`

``IsPlaceEnabled()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.AvatarChatService:IsUniverseEnabled`

``IsUniverseEnabled()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.AvatarChatService:PollClientFeatures`

``PollClientFeatures()`` → `int`
   {security: RobloxScriptSecurity}

### `Class.AvatarChatService:PollServerFeatures`

``PollServerFeatures()`` → `int`
   {security: RobloxScriptSecurity}

### `Class.AvatarChatService:deviceMeetsRequirementsForFeature`

``deviceMeetsRequirementsForFeature(feature: `Enum.DeviceFeatureType`)`` → `bool`
   {security: RobloxScriptSecurity}
