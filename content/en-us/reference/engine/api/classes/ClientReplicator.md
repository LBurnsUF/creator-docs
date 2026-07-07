---
title: ClientReplicator
type: class
superclass: NetworkReplicator
tags: [NotCreatable, NotReplicated]
---

# ClientReplicator

**Inherits from:** `Class.NetworkReplicator` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Methods

### `Class.ClientReplicator:IsStreamedOut`

``IsStreamedOut(instance: `Class.Instance`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.ClientReplicator:RequestRCCProfilerData`

``RequestRCCProfilerData(frameRate: `int`, timeFrame: `int`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.ClientReplicator:RequestServerStats`

``RequestServerStats(request: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.ClientReplicator.RCCProfilerDataComplete`

Fires with: (success: `bool`, message: `string`)

### `Class.ClientReplicator.StatsReceived`

Fires with: (stats: `Dictionary`)
