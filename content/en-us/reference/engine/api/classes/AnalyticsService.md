---
title: AnalyticsService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# AnalyticsService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **ApiKey**: `string` [Deprecated] (Security: Read=LocalUserSecurity, Write=LocalUserSecurity)

## Methods

- **FireCustomEvent**(`player: Instance`, `eventCategory: string`, `customData: Variant`) -> `null` [Deprecated]
- **FireEvent**(`category: string`, `value: Variant`) -> `null` [Deprecated]
- **FireInGameEconomyEvent**(`player: Instance`, `itemName: string`, `economyAction: AnalyticsEconomyAction`, `itemCategory: string`, `amount: int`, `currency: string`, `location: Variant`, `customData: Variant`) -> `null` [Deprecated]
- **FireLogEvent**(`player: Instance`, `logLevel: AnalyticsLogLevel`, `message: string`, `debugInfo: Variant`, `customData: Variant`) -> `null` [Deprecated]
- **FirePlayerProgressionEvent**(`player: Instance`, `category: string`, `progressionStatus: AnalyticsProgressionStatus`, `location: Variant`, `statistics: Variant`, `customData: Variant`) -> `null` [Deprecated]
- **GetDurationLoggerTimestamp**() -> `int`
- **GetPlayerSegmentsAsync**(`player: Player`) -> `Dictionary` [Yields]
- **LogCustomEvent**(`player: Player`, `eventName: string`, `value: double = 1`, `customFields: Dictionary = nil`) -> `null`
- **LogEconomyEvent**(`player: Player`, `flowType: AnalyticsEconomyFlowType`, `currencyType: string`, `amount: float`, `endingBalance: float`, `transactionType: string`, `itemSku: string = `, `customFields: Dictionary = nil`) -> `null`
- **LogFunnelStepEvent**(`player: Player`, `funnelName: string`, `funnelSessionId: string = `, `step: int = 1`, `stepName: string = `, `customFields: Dictionary = nil`) -> `null`
- **LogOnboardingFunnelStepEvent**(`player: Player`, `step: int`, `stepName: string = `, `customFields: Dictionary = nil`) -> `null`
- **LogProgressionCompleteEvent**(`player: Player`, `progressionPathName: string`, `level: int`, `levelName: string = `, `customFields: Dictionary = nil`) -> `null`
- **LogProgressionEvent**(`player: Player`, `progressionPathName: string`, `status: AnalyticsProgressionType`, `level: int`, `levelName: string = `, `customFields: Dictionary = nil`) -> `null`
- **LogProgressionFailEvent**(`player: Player`, `progressionPathName: string`, `level: int`, `levelName: string = `, `customFields: Dictionary = nil`) -> `null`
- **LogProgressionStartEvent**(`player: Player`, `progressionPathName: string`, `level: int`, `levelName: string = `, `customFields: Dictionary = nil`) -> `null`
