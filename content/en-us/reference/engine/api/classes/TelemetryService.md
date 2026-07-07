---
title: TelemetryService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# TelemetryService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **LogCounter**(`config: Dictionary`, `data: Dictionary?`, `value: float = 1`) -> `Variant`
- **LogDurationEvent**(`key: string`) -> `Variant`
- **LogDurationEventWithTimestamp**(`key: string`, `timestamp: int64`) -> `Variant`
- **LogEvent**(`config: Dictionary`, `data: Dictionary = nil`) -> `Variant`
- **LogStat**(`config: Dictionary`, `data: Dictionary?`, `value: float`) -> `Variant`
