---
title: LogReporterService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# LogReporterService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.LogReporterService:ReportLog`

``ReportLog(fingerprint: `string`, uuid: `string`, desc: `string`, attributes: `Dictionary`, annotations: `Dictionary`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.LogReporterService:ReportMultipleLogs`

``ReportMultipleLogs(fingerprint: `string`, uuid: `string`, desc: `string`, attributes: `Dictionary`, annotations: `Dictionary`, numLogs: `int`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.LogReporterService:SubmitStratusBugReport`

``SubmitStratusBugReport(description: `string`, username: `string`)`` -> `bool`
   {security: RobloxScriptSecurity}
