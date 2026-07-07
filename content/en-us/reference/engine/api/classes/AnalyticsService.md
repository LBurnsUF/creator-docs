---
title: AnalyticsService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# AnalyticsService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.AnalyticsService.ApiKey` | `string` | [Deprecated] {security: LocalUserSecurity} |

## Methods

### `Class.AnalyticsService:FireCustomEvent`

``FireCustomEvent(player: `Class.Instance`, eventCategory: `string`, customData: `Variant`)`` → `null`
  [Deprecated]

### `Class.AnalyticsService:FireEvent`

``FireEvent(category: `string`, value: `Variant`)`` → `null`
  [Deprecated]

### `Class.AnalyticsService:FireInGameEconomyEvent`

``FireInGameEconomyEvent(player: `Class.Instance`, itemName: `string`, economyAction: `Enum.AnalyticsEconomyAction`, itemCategory: `string`, amount: `int`, currency: `string`, location: `Variant`, customData: `Variant`)`` → `null`
  [Deprecated]

### `Class.AnalyticsService:FireLogEvent`

``FireLogEvent(player: `Class.Instance`, logLevel: `Enum.AnalyticsLogLevel`, message: `string`, debugInfo: `Variant`, customData: `Variant`)`` → `null`
  [Deprecated]

### `Class.AnalyticsService:FirePlayerProgressionEvent`

``FirePlayerProgressionEvent(player: `Class.Instance`, category: `string`, progressionStatus: `Enum.AnalyticsProgressionStatus`, location: `Variant`, statistics: `Variant`, customData: `Variant`)`` → `null`
  [Deprecated]

### `Class.AnalyticsService:GetDurationLoggerTimestamp`

``GetDurationLoggerTimestamp()`` → `int`

### `Class.AnalyticsService:GetPlayerSegmentsAsync`

``GetPlayerSegmentsAsync(player: `Class.Player`)`` → `Dictionary`
  [Yields]

### `Class.AnalyticsService:LogCustomEvent`

``LogCustomEvent(player: `Class.Player`, eventName: `string`, value: `double`, customFields: `Dictionary`)`` → `null`

### `Class.AnalyticsService:LogEconomyEvent`

``LogEconomyEvent(player: `Class.Player`, flowType: `Enum.AnalyticsEconomyFlowType`, currencyType: `string`, amount: `float`, endingBalance: `float`, transactionType: `string`, itemSku: `string`, customFields: `Dictionary`)`` → `null`

### `Class.AnalyticsService:LogFunnelStepEvent`

``LogFunnelStepEvent(player: `Class.Player`, funnelName: `string`, funnelSessionId: `string`, step: `int`, stepName: `string`, customFields: `Dictionary`)`` → `null`

### `Class.AnalyticsService:LogOnboardingFunnelStepEvent`

``LogOnboardingFunnelStepEvent(player: `Class.Player`, step: `int`, stepName: `string`, customFields: `Dictionary`)`` → `null`

### `Class.AnalyticsService:LogProgressionCompleteEvent`

``LogProgressionCompleteEvent(player: `Class.Player`, progressionPathName: `string`, level: `int`, levelName: `string`, customFields: `Dictionary`)`` → `null`

### `Class.AnalyticsService:LogProgressionEvent`

``LogProgressionEvent(player: `Class.Player`, progressionPathName: `string`, status: `Enum.AnalyticsProgressionType`, level: `int`, levelName: `string`, customFields: `Dictionary`)`` → `null`

### `Class.AnalyticsService:LogProgressionFailEvent`

``LogProgressionFailEvent(player: `Class.Player`, progressionPathName: `string`, level: `int`, levelName: `string`, customFields: `Dictionary`)`` → `null`

### `Class.AnalyticsService:LogProgressionStartEvent`

``LogProgressionStartEvent(player: `Class.Player`, progressionPathName: `string`, level: `int`, levelName: `string`, customFields: `Dictionary`)`` → `null`
