---
title: AvatarChatService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# AvatarChatService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **ClientFeatures**: `int` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **ClientFeaturesInitialized**: `bool` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **ServerFeatures**: `int` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxSecurity)

## Methods

- **DebugCounterGet**(`label: string`, `playerId: int64`) -> `int64`
- **EnableVoice**() -> `bool`
- **GetClientFeaturesAsync**() -> `int` [Yields]
- **GetServerFeaturesAsync**() -> `int` [Yields]
- **IsEnabled**(`mask: int`, `feature: AvatarChatServiceFeature`) -> `bool`
- **IsPlaceEnabled**() -> `bool`
- **IsUniverseEnabled**() -> `bool`
- **PollClientFeatures**() -> `int`
- **PollServerFeatures**() -> `int`
- **deviceMeetsRequirementsForFeature**(`feature: DeviceFeatureType`) -> `bool`
