---
title: RbxAnalyticsService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# RbxAnalyticsService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.RbxAnalyticsService:AddGlobalPointsField`

``AddGlobalPointsField(key: `string`, value: `int`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.RbxAnalyticsService:AddGlobalPointsTag`

``AddGlobalPointsTag(key: `string`, value: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.RbxAnalyticsService:DEPRECATED_TrackEvent`

``DEPRECATED_TrackEvent(category: `string`, action: `string`, label: `string`, value: `int64`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.RbxAnalyticsService:DEPRECATED_TrackEventWithArgs`

``DEPRECATED_TrackEventWithArgs(category: `string`, action: `string`, label: `string`, args: `Dictionary`, value: `int64`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.RbxAnalyticsService:GetClientId`

``GetClientId()`` → `string`
   {security: RobloxScriptSecurity}

### `Class.RbxAnalyticsService:GetPlaySessionId`

``GetPlaySessionId()`` → `string`
   {security: RobloxScriptSecurity}

### `Class.RbxAnalyticsService:GetSessionId`

``GetSessionId()`` → `string`
   {security: RobloxScriptSecurity}

### `Class.RbxAnalyticsService:ReleaseRBXEventStream`

``ReleaseRBXEventStream(target: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.RbxAnalyticsService:RemoveGlobalPointsField`

``RemoveGlobalPointsField(key: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.RbxAnalyticsService:RemoveGlobalPointsTag`

``RemoveGlobalPointsTag(key: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.RbxAnalyticsService:ReportCounter`

``ReportCounter(counterName: `string`, amount: `int`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.RbxAnalyticsService:ReportInfluxSeries`

``ReportInfluxSeries(seriesName: `string`, points: `Dictionary`, throttlingPercentage: `int`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.RbxAnalyticsService:ReportStats`

``ReportStats(category: `string`, value: `float`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.RbxAnalyticsService:ReportToDiagByCountryCode`

``ReportToDiagByCountryCode(featureName: `string`, measureName: `string`, seconds: `double`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.RbxAnalyticsService:SendEventDeferred`

``SendEventDeferred(target: `string`, eventContext: `string`, eventName: `string`, additionalArgs: `Dictionary`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.RbxAnalyticsService:SendEventImmediately`

``SendEventImmediately(target: `string`, eventContext: `string`, eventName: `string`, additionalArgs: `Dictionary`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.RbxAnalyticsService:SetRBXEvent`

``SetRBXEvent(target: `string`, eventContext: `string`, eventName: `string`, additionalArgs: `Dictionary`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.RbxAnalyticsService:SetRBXEventStream`

``SetRBXEventStream(target: `string`, eventContext: `string`, eventName: `string`, additionalArgs: `Dictionary`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.RbxAnalyticsService:TrackEvent`

``TrackEvent(category: `string`, action: `string`, label: `string`, value: `int64`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.RbxAnalyticsService:TrackEventWithArgs`

``TrackEventWithArgs(category: `string`, action: `string`, label: `string`, args: `Dictionary`, value: `int64`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.RbxAnalyticsService:UpdateHeartbeatObject`

``UpdateHeartbeatObject(args: `Dictionary`)`` → `null`
   {security: RobloxScriptSecurity}
