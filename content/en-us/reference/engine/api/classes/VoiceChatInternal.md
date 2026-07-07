---
title: VoiceChatInternal
type: class
superclass: Instance
tags: [NotCreatable, Service, NotBrowsable]
---

# VoiceChatInternal

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotBrowsable

## Properties

- **VoiceChatState**: `VoiceChatState` [Hidden] [ReadOnly] [NotReplicated] [Deprecated]

## Methods

- **GetAndClearCallFailureMessage**() -> `string` [Deprecated]
- **GetAudioProcessingSettings**() -> `Tuple` [Deprecated]
- **GetChannelId**() -> `string`
- **GetGroupId**() -> `string`
- **GetMicDevices**() -> `Tuple` [Deprecated]
- **GetParticipants**() -> `Array` [Deprecated]
- **GetSessionId**() -> `string`
- **GetVoiceChatApiVersion**() -> `int` [Deprecated]
- **GetVoiceChatAvailable**() -> `int` [Deprecated]
- **GetVoiceExperienceId**() -> `string`
- **IsContextVoiceEnabled**() -> `bool`
- **IsPublishPaused**() -> `bool` [Deprecated]
- **IsSubscribePaused**(`userId: int64`) -> `bool` [Deprecated]
- **IsVoiceEnabledForUserIdAsync**(`userId: int64`) -> `bool` [Yields]
- **JoinByGroupId**(`groupId: string`, `isMicMuted: bool = false`) -> `bool` [Deprecated]
- **JoinByGroupIdToken**(`groupId: string`, `isMicMuted: bool`, `isRetry: bool = false`) -> `bool` [Deprecated]
- **Leave**() -> `null` [Deprecated]
- **LogPublisherWebRTCStats**() -> `bool`
- **LogSubscriptionWebRTCStats**() -> `bool`
- **PublishPause**(`paused: bool`) -> `bool` [Deprecated]
- **SetMicDevice**(`micDeviceName: string`, `micDeviceGuid: string`) -> `null` [Deprecated]
- **SubscribeBlock**(`userId: int64`) -> `bool`
- **SubscribePause**(`userId: int64`, `paused: bool`) -> `bool` [Deprecated]
- **SubscribePauseAll**(`paused: bool`) -> `bool` [Deprecated]
- **SubscribeRetry**(`userId: int64`) -> `bool`
- **SubscribeUnblock**(`userId: int64`) -> `bool`

## Events

- **LocalPlayerModerated**()
- **ParticipantsStateChanged**(`participantsLeft: Array`, `participantsJoined: Array`, `updatedStates: Array`) [Deprecated]
- **PlayerMicActivitySignalChange**(`activityInfo: Dictionary`) [Deprecated]
- **StateChanged**(`old: VoiceChatState`, `new: VoiceChatState`) [Deprecated]
- **TempSetMicMutedToggleMic**()
