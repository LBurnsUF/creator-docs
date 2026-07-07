---
title: ClientReplicator
type: class
superclass: NetworkReplicator
tags: [NotCreatable, NotReplicated]
---

# ClientReplicator

**Inherits**: NetworkReplicator > Instance > Object

**Tags**: NotCreatable, NotReplicated

## Methods

- **IsStreamedOut**(`instance: Instance`) -> `bool`
- **RequestRCCProfilerData**(`frameRate: int`, `timeFrame: int`) -> `null`
- **RequestServerStats**(`request: bool`) -> `null`

## Events

- **RCCProfilerDataComplete**(`success: bool`, `message: string`)
- **StatsReceived**(`stats: Dictionary`)
