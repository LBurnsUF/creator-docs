---
title: VoiceChatInternal
type: class
superclass: Instance
tags: [NotCreatable, Service, NotBrowsable]
---

# VoiceChatInternal

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotBrowsable]

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.VoiceChatInternal.VoiceChatState` | `Enum.VoiceChatState` | [Hidden] [ReadOnly] [NotReplicated] [Deprecated] |

## Methods

### `Class.VoiceChatInternal:GetAndClearCallFailureMessage`

``GetAndClearCallFailureMessage()`` -> `string`
  [Deprecated] {security: RobloxScriptSecurity}

### `Class.VoiceChatInternal:GetAudioProcessingSettings`

``GetAudioProcessingSettings()`` -> `Tuple`
  [Deprecated]

### `Class.VoiceChatInternal:GetChannelId`

``GetChannelId()`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatInternal:GetGroupId`

``GetGroupId()`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatInternal:GetMicDevices`

``GetMicDevices()`` -> `Tuple`
  [Deprecated]

### `Class.VoiceChatInternal:GetParticipants`

``GetParticipants()`` -> `Array`
  [Deprecated]

### `Class.VoiceChatInternal:GetSessionId`

``GetSessionId()`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatInternal:GetVoiceChatApiVersion`

``GetVoiceChatApiVersion()`` -> `int`
  [Deprecated]

### `Class.VoiceChatInternal:GetVoiceChatAvailable`

``GetVoiceChatAvailable()`` -> `int`
  [Deprecated]

### `Class.VoiceChatInternal:GetVoiceExperienceId`

``GetVoiceExperienceId()`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatInternal:IsContextVoiceEnabled`

``IsContextVoiceEnabled()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatInternal:IsPublishPaused`

``IsPublishPaused()`` -> `bool`
  [Deprecated]

### `Class.VoiceChatInternal:IsSubscribePaused`

``IsSubscribePaused(userId: `int64`)`` -> `bool`
  [Deprecated]

### `Class.VoiceChatInternal:IsVoiceEnabledForUserIdAsync`

``IsVoiceEnabledForUserIdAsync(userId: `int64`)`` -> `bool`
  [Yields]

### `Class.VoiceChatInternal:JoinByGroupId`

``JoinByGroupId(groupId: `string`, isMicMuted: `bool`)`` -> `bool`
  [Deprecated]

### `Class.VoiceChatInternal:JoinByGroupIdToken`

``JoinByGroupIdToken(groupId: `string`, isMicMuted: `bool`, isRetry: `bool`)`` -> `bool`
  [Deprecated]

### `Class.VoiceChatInternal:Leave`

``Leave()`` -> `null`
  [Deprecated]

### `Class.VoiceChatInternal:LogPublisherWebRTCStats`

``LogPublisherWebRTCStats()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatInternal:LogSubscriptionWebRTCStats`

``LogSubscriptionWebRTCStats()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatInternal:PublishPause`

``PublishPause(paused: `bool`)`` -> `bool`
  [Deprecated]

### `Class.VoiceChatInternal:SetMicDevice`

``SetMicDevice(micDeviceName: `string`, micDeviceGuid: `string`)`` -> `null`
  [Deprecated]

### `Class.VoiceChatInternal:SubscribeBlock`

``SubscribeBlock(userId: `int64`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatInternal:SubscribePause`

``SubscribePause(userId: `int64`, paused: `bool`)`` -> `bool`
  [Deprecated]

### `Class.VoiceChatInternal:SubscribePauseAll`

``SubscribePauseAll(paused: `bool`)`` -> `bool`
  [Deprecated]

### `Class.VoiceChatInternal:SubscribeRetry`

``SubscribeRetry(userId: `int64`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.VoiceChatInternal:SubscribeUnblock`

``SubscribeUnblock(userId: `int64`)`` -> `bool`
   {security: RobloxScriptSecurity}

## Events

### `Class.VoiceChatInternal.LocalPlayerModerated`

Fires with: ()

### `Class.VoiceChatInternal.ParticipantsStateChanged`

Fires with: (participantsLeft: `Array`, participantsJoined: `Array`, updatedStates: `Array`)
  [Deprecated]

### `Class.VoiceChatInternal.PlayerMicActivitySignalChange`

Fires with: (activityInfo: `Dictionary`)
  [Deprecated]

### `Class.VoiceChatInternal.StateChanged`

Fires with: (old: `Enum.VoiceChatState`, new: `Enum.VoiceChatState`)
  [Deprecated]

### `Class.VoiceChatInternal.TempSetMicMutedToggleMic`

Fires with: ()
