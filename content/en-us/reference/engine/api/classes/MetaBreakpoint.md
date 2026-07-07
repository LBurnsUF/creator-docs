---
title: MetaBreakpoint
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# MetaBreakpoint

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.MetaBreakpoint.Condition` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.MetaBreakpoint.ContinueExecution` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.MetaBreakpoint.Enabled` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.MetaBreakpoint.Id` | `int` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.MetaBreakpoint.IsLogpoint` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.MetaBreakpoint.Line` | `int` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.MetaBreakpoint.LogMessage` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.MetaBreakpoint.RemoveOnHit` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.MetaBreakpoint.Script` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.MetaBreakpoint.Valid` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |

## Methods

### `Class.MetaBreakpoint:GetContextBreakpoints`

``GetContextBreakpoints()`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.MetaBreakpoint:Remove`

``Remove(status: `Datatype.Function`)`` → `int`
   {security: RobloxScriptSecurity}

### `Class.MetaBreakpoint:SetChildBreakpointEnabledByScriptAndContext`

``SetChildBreakpointEnabledByScriptAndContext(script: `string`, contextGST: `int`, enabled: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.MetaBreakpoint:SetContextEnabled`

``SetContextEnabled(context: `int`, enabled: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.MetaBreakpoint:SetContinueExecution`

``SetContinueExecution(enabled: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.MetaBreakpoint:SetEnabled`

``SetEnabled(enabled: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.MetaBreakpoint:SetLine`

``SetLine(line: `int`, status: `Datatype.Function`)`` → `int`
   {security: RobloxScriptSecurity}

### `Class.MetaBreakpoint:SetRemoveOnHit`

``SetRemoveOnHit(enabled: `bool`)`` → `null`
   {security: RobloxScriptSecurity}
