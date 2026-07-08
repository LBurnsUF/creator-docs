---
title: DebuggerUIService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# DebuggerUIService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.DebuggerUIService:EditBreakpoint`

``EditBreakpoint(metaBreakpointId: `int`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.DebuggerUIService:EditWatch`

``EditWatch(expression: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.DebuggerUIService:IsConnectionForPlayDataModel`

``IsConnectionForPlayDataModel(debuggerConnectionId: `int`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.DebuggerUIService:OpenExceptionMessagePopup`

``OpenExceptionMessagePopup(exceptionMessage: `string`, pausedLine: `int`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.DebuggerUIService:OpenScriptAtLine`

``OpenScriptAtLine(guid: `string`, debuggerConnectionId: `int`, line: `int`, showErrorOnFail: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.DebuggerUIService:Pause`

``Pause()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.DebuggerUIService:RemoveScriptLineMarkers`

``RemoveScriptLineMarkers(debuggerConnectionId: `int`, allMarkers: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.DebuggerUIService:Resume`

``Resume()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.DebuggerUIService:SetCurrentThreadId`

``SetCurrentThreadId(debuggerThreadId: `int`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.DebuggerUIService:SetScriptLineMarker`

``SetScriptLineMarker(guid: `string`, debuggerConnectionId: `int`, line: `int`, lineMarkerType: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.DebuggerUIService:SetWatchExpressions`

``SetWatchExpressions(expressions: `Array`)`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.DebuggerUIService.ExpressionAdded`

Fires with: (expression: `string`)

### `Class.DebuggerUIService.ExpressionsCleared`

Fires with: ()
