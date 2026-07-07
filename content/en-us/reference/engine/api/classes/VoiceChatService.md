---
title: VoiceChatService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# VoiceChatService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **DefaultDistanceAttenuation**: `VoiceChatDistanceAttenuationType` (Security: Read=PluginSecurity, Write=PluginSecurity)
- **EnableDefaultVoice**: `bool` (Security: Read=PluginSecurity, Write=PluginSecurity)
- **UseAudioApi**: `AudioApiRollout` (Security: Read=PluginSecurity, Write=PluginSecurity)
- **UseNewAudioApi**: `bool` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **UseNewControlPaths**: `bool` [Hidden] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **UseNewJoinFlow**: `bool` [Hidden] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **UseStreamSwitching**: `bool` [Hidden] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **VoiceChatEnabledForPlaceOnRcc**: `bool` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **VoiceChatEnabledForUniverseOnRcc**: `bool` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **GetChatGroupsAsync**(`players: Instances`) -> `Array` [Yields]
- **IsVoiceEnabledForUserIdAsync**(`userId: User`) -> `bool` [Yields]
- **getInternalChannelId**() -> `string`
- **getInternalGroupId**() -> `string`
- **getInternalPublishPause**() -> `bool`
- **getInternalSessionId**() -> `string`
- **getInternalSubscribePause**(`userId: int64`) -> `bool`
- **getInternalSubscribePauseAll**() -> `bool`
- **getInternalVoiceChatApiVersion**() -> `int`
- **isInternalPublishPaused**() -> `bool`
- **joinVoice**() -> `null`
- **lastVoiceChatStats**() -> `Dictionary`
- **leaveVoice**(`leaveReason: VoiceClientLeaveReasons = LuaInitiated`) -> `null`
- **notifyServerACSCleanup**() -> `null`
- **rejoinVoice**() -> `null`

## Events

- **VoiceChatStatsCollected**()
