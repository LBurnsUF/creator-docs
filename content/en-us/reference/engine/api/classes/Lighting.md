---
title: Lighting
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# Lighting

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **Ambient**: `Color3`
- **Brightness**: `float`
- **ClockTime**: `float` [NotReplicated]
- **ColorShift_Bottom**: `Color3`
- **ColorShift_Top**: `Color3`
- **EnvironmentDiffuseScale**: `float`
- **EnvironmentSpecularScale**: `float`
- **ExposureCompensation**: `float`
- **ExtendLightRangeTo120**: `RolloutState` [NotScriptable]
- **FogColor**: `Color3`
- **FogEnd**: `float`
- **FogStart**: `float`
- **GeographicLatitude**: `float`
- **GlobalShadows**: `bool`
- **LightingStyle**: `LightingStyle` (Security: Read=None, Write=RobloxScriptSecurity)
- **OutdoorAmbient**: `Color3`
- **Outlines**: `bool` [Deprecated]
- **PrioritizeLightingQuality**: `bool` (Security: Read=None, Write=RobloxScriptSecurity)
- **ShadowColor**: `Color3` [NotReplicated] [Deprecated]
- **ShadowSoftness**: `float`
- **Technology**: `Technology` (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **TimeOfDay**: `string`

## Methods

- **GetMinutesAfterMidnight**() -> `double`
- **GetMoonDirection**() -> `Vector3`
- **GetMoonPhase**() -> `float`
- **GetSunDirection**() -> `Vector3`
- **SetMinutesAfterMidnight**(`minutes: double`) -> `null`
- **getMinutesAfterMidnight**() -> `double` [Deprecated]
- **setMinutesAfterMidnight**(`minutes: double`) -> `null` [Deprecated]

## Events

- **LightingChanged**(`skyChanged: bool`)
