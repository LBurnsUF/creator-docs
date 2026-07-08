---
title: ScriptEditorService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ScriptEditorService

This service is used for interacting with `Class.ScriptDocument` instances.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

This service is used for interacting with `Class.ScriptDocument` instances.

## Methods

### `Class.ScriptEditorService:DeregisterAutocompleteCallback`

``DeregisterAutocompleteCallback(name: `string`)`` -> `null`
   {security: PluginSecurity}

### `Class.ScriptEditorService:DeregisterScriptAnalysisCallback`

``DeregisterScriptAnalysisCallback(name: `string`)`` -> `null`
   {security: PluginSecurity}

### `Class.ScriptEditorService:EditSourceAsyncWithRanges`

``EditSourceAsyncWithRanges(script: `Class.LuaSourceContainer`, newText: `string`, startLine: `int`, startCharacter: `int`, endLine: `int`, endCharacter: `int`)`` -> `Tuple`
  [Yields] {security: RobloxScriptSecurity}

### `Class.ScriptEditorService:FindScriptDocument`

``FindScriptDocument(script: `Class.LuaSourceContainer`)`` -> `Class.ScriptDocument`
   {security: PluginSecurity}

### `Class.ScriptEditorService:ForceReloadSource`

``ForceReloadSource(uri: `string`, newsrc: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.ScriptEditorService:GetEditorSource`

``GetEditorSource(script: `Class.LuaSourceContainer`)`` -> `string`
   {security: PluginSecurity}

### `Class.ScriptEditorService:GetScriptDocuments`

``GetScriptDocuments()`` -> `Datatype.Instances`
   {security: PluginSecurity}

### `Class.ScriptEditorService:IsAutocompleteCallbackRegistered`

``IsAutocompleteCallbackRegistered(name: `string`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.ScriptEditorService:IsScriptAnalysisCallbackRegistered`

``IsScriptAnalysisCallbackRegistered(name: `string`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.ScriptEditorService:OpenScriptDocumentAsync`

``OpenScriptDocumentAsync(script: `Class.LuaSourceContainer`, options: `Dictionary`)`` -> `Tuple`
  [Yields] {security: PluginSecurity}

### `Class.ScriptEditorService:RegisterAutocompleteCallback`

``RegisterAutocompleteCallback(name: `string`, priority: `int`, callbackFunction: `Datatype.Function`)`` -> `null`
   {security: PluginSecurity}

### `Class.ScriptEditorService:RegisterScriptAnalysisCallback`

``RegisterScriptAnalysisCallback(name: `string`, priority: `int`, callbackFunction: `Datatype.Function`)`` -> `null`
   {security: PluginSecurity}

### `Class.ScriptEditorService:StripComments`

``StripComments(code: `string`)`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.ScriptEditorService:UpdateSourceAsync`

``UpdateSourceAsync(script: `Class.LuaSourceContainer`, callback: `Datatype.Function`)`` -> `null`
  [Yields] {security: PluginSecurity}

## Events

### `Class.ScriptEditorService.TextDocumentDidChange`

Fires with: (document: `Class.ScriptDocument`, changesArray: `Variant`)

### `Class.ScriptEditorService.TextDocumentDidClose`

Fires with: (oldDocument: `Class.ScriptDocument`)

### `Class.ScriptEditorService.TextDocumentDidOpen`

Fires with: (newDocument: `Class.ScriptDocument`)
