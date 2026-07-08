---
title: ScriptContext
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ScriptContext

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

This service controls all `Class.BaseScript` objects. Most of the properties
and methods of this service are locked for internal use.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ScriptContext.ScriptsDisabled` | `bool` | [Hidden] {security: LocalUserSecurity} |

## Methods

### `Class.ScriptContext:AddCoreScriptLocal`

``AddCoreScriptLocal(name: `string`, parent: `Class.Instance`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.ScriptContext:CompressLuaApp`

``CompressLuaApp()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.ScriptContext:EnableCoverage`

``EnableCoverage(instance: `Class.Instance`)`` -> `null`

### `Class.ScriptContext:GetCoverageStats`

``GetCoverageStats()`` -> `Array`

### `Class.ScriptContext:GetLuauHeapInstanceReferenceReport`

``GetLuauHeapInstanceReferenceReport(target: `string`)`` -> `Dictionary`
  [CustomLuaState] {security: RobloxScriptSecurity}

### `Class.ScriptContext:GetLuauHeapMemoryReport`

``GetLuauHeapMemoryReport(target: `string`)`` -> `Dictionary`
  [CustomLuaState] {security: RobloxScriptSecurity}

### `Class.ScriptContext:ReportLuaRequireCount`

``ReportLuaRequireCount()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.ScriptContext:SetTimeout`

``SetTimeout(seconds: `double`)`` -> `null`
   {security: PluginSecurity}

## Events

### `Class.ScriptContext.Error`

Fires with: (message: `string`, stackTrace: `string`, script: `Class.Instance`)

### `Class.ScriptContext.ErrorDetailed`

Fires with: (message: `string`, stackTrace: `string`, script: `Class.Instance`, details: `string`, securityLevel: `int`, messageId: `string`)
