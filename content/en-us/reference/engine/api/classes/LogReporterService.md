---
title: LogReporterService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# LogReporterService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **ReportLog**(`fingerprint: string`, `uuid: string`, `desc: string`, `attributes: Dictionary`, `annotations: Dictionary`) -> `bool`
- **ReportMultipleLogs**(`fingerprint: string`, `uuid: string`, `desc: string`, `attributes: Dictionary`, `annotations: Dictionary`, `numLogs: int`) -> `bool`
- **SubmitStratusBugReport**(`description: string`, `username: string`) -> `bool`
