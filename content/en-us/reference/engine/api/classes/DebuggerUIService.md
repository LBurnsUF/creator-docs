---
title: DebuggerUIService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# DebuggerUIService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **EditBreakpoint**(`metaBreakpointId: int`) -> `null`
- **EditWatch**(`expression: string`) -> `null`
- **IsConnectionForPlayDataModel**(`debuggerConnectionId: int`) -> `bool`
- **OpenExceptionMessagePopup**(`exceptionMessage: string`, `pausedLine: int`) -> `null`
- **OpenScriptAtLine**(`guid: string`, `debuggerConnectionId: int`, `line: int`, `showErrorOnFail: bool`) -> `null`
- **Pause**() -> `null`
- **RemoveScriptLineMarkers**(`debuggerConnectionId: int`, `allMarkers: bool`) -> `null`
- **Resume**() -> `null`
- **SetCurrentThreadId**(`debuggerThreadId: int`) -> `null`
- **SetScriptLineMarker**(`guid: string`, `debuggerConnectionId: int`, `line: int`, `lineMarkerType: bool`) -> `null`
- **SetWatchExpressions**(`expressions: Array`) -> `null`

## Events

- **ExpressionAdded**(`expression: string`)
- **ExpressionsCleared**()
