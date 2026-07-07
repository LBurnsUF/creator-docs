---
title: RbxAnalyticsService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# RbxAnalyticsService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **AddGlobalPointsField**(`key: string`, `value: int`) -> `null`
- **AddGlobalPointsTag**(`key: string`, `value: string`) -> `null`
- **DEPRECATED_TrackEvent**(`category: string`, `action: string`, `label: string`, `value: int64 = 0`) -> `null`
- **DEPRECATED_TrackEventWithArgs**(`category: string`, `action: string`, `label: string`, `args: Dictionary`, `value: int64 = 0`) -> `null`
- **GetClientId**() -> `string`
- **GetPlaySessionId**() -> `string`
- **GetSessionId**() -> `string`
- **ReleaseRBXEventStream**(`target: string`) -> `null`
- **RemoveGlobalPointsField**(`key: string`) -> `null`
- **RemoveGlobalPointsTag**(`key: string`) -> `null`
- **ReportCounter**(`counterName: string`, `amount: int = 1`) -> `null`
- **ReportInfluxSeries**(`seriesName: string`, `points: Dictionary`, `throttlingPercentage: int`) -> `null`
- **ReportStats**(`category: string`, `value: float`) -> `null`
- **ReportToDiagByCountryCode**(`featureName: string`, `measureName: string`, `seconds: double`) -> `null`
- **SendEventDeferred**(`target: string`, `eventContext: string`, `eventName: string`, `additionalArgs: Dictionary`) -> `null`
- **SendEventImmediately**(`target: string`, `eventContext: string`, `eventName: string`, `additionalArgs: Dictionary`) -> `null`
- **SetRBXEvent**(`target: string`, `eventContext: string`, `eventName: string`, `additionalArgs: Dictionary`) -> `null`
- **SetRBXEventStream**(`target: string`, `eventContext: string`, `eventName: string`, `additionalArgs: Dictionary`) -> `null`
- **TrackEvent**(`category: string`, `action: string`, `label: string`, `value: int64 = 0`) -> `null`
- **TrackEventWithArgs**(`category: string`, `action: string`, `label: string`, `args: Dictionary`, `value: int64 = 0`) -> `null`
- **UpdateHeartbeatObject**(`args: Dictionary`) -> `null`
