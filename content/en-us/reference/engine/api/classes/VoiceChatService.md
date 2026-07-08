---
title: VoiceChatService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# VoiceChatService

**VoiceChatService** is responsible for voice chat's high-level functionality.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

**VoiceChatService** is responsible for voice chat's high-level functionality.
This mostly consists of configuration options, and functions that are not
specifically-controlled by more-specific instances.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.VoiceChatService.DefaultDistanceAttenuation` | `Enum.VoiceChatDistanceAttenuationType` |  {security: PluginSecurity} |
| `Class.VoiceChatService.EnableDefaultVoice` | `bool` |  {security: PluginSecurity} |
| `Class.VoiceChatService.UseAudioApi` | `Enum.AudioApiRollout` |  {security: PluginSecurity} |
| `Class.VoiceChatService.UseNewAudioApi` | `bool` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.VoiceChatService.UseNewControlPaths` | `bool` | [Hidden] {security: RobloxSecurity} |
| `Class.VoiceChatService.UseNewJoinFlow` | `bool` | [Hidden] {security: RobloxSecurity} |
| `Class.VoiceChatService.UseStreamSwitching` | `bool` | [Hidden] {security: RobloxSecurity} |
| `Class.VoiceChatService.VoiceChatEnabledForPlaceOnRcc` | `bool` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.VoiceChatService.VoiceChatEnabledForUniverseOnRcc` | `bool` | [Hidden] {security: RobloxScriptSecurity} |

## Methods

### `Class.VoiceChatService:GetChatGroupsAsync`

``GetChatGroupsAsync(players: `Datatype.Instances`)`` -> `Array`
  [Yields]

### `Class.VoiceChatService:IsVoiceEnabledForUserIdAsync`

``IsVoiceEnabledForUserIdAsync(userId: `Datatype.User`)`` -> `bool`
  [Yields]

### `Class.VoiceChatService:getInternalChannelId`

``getInternalChannelId()`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatService:getInternalGroupId`

``getInternalGroupId()`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatService:getInternalPublishPause`

``getInternalPublishPause()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatService:getInternalSessionId`

``getInternalSessionId()`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatService:getInternalSubscribePause`

``getInternalSubscribePause(userId: `int64`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatService:getInternalSubscribePauseAll`

``getInternalSubscribePauseAll()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatService:getInternalVoiceChatApiVersion`

``getInternalVoiceChatApiVersion()`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatService:isInternalPublishPaused`

``isInternalPublishPaused()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatService:joinVoice`

``joinVoice()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatService:lastVoiceChatStats`

``lastVoiceChatStats()`` -> `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatService:leaveVoice`

``leaveVoice(leaveReason: `Enum.VoiceClientLeaveReasons`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatService:notifyServerACSCleanup`

``notifyServerACSCleanup()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatService:rejoinVoice`

``rejoinVoice()`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.VoiceChatService.VoiceChatStatsCollected`

Fires with: ()
