---
title: ScriptEditorService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ScriptEditorService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **DeregisterAutocompleteCallback**(`name: string`) -> `null`
- **DeregisterScriptAnalysisCallback**(`name: string`) -> `null`
- **EditSourceAsyncWithRanges**(`script: LuaSourceContainer`, `newText: string`, `startLine: int`, `startCharacter: int`, `endLine: int`, `endCharacter: int`) -> `Tuple` [Yields]
- **FindScriptDocument**(`script: LuaSourceContainer`) -> `ScriptDocument`
- **ForceReloadSource**(`uri: string`, `newsrc: string`) -> `null`
- **GetEditorSource**(`script: LuaSourceContainer`) -> `string`
- **GetScriptDocuments**() -> `Instances`
- **IsAutocompleteCallbackRegistered**(`name: string`) -> `bool`
- **IsScriptAnalysisCallbackRegistered**(`name: string`) -> `bool`
- **OpenScriptDocumentAsync**(`script: LuaSourceContainer`, `options: Dictionary = nil`) -> `Tuple` [Yields]
- **RegisterAutocompleteCallback**(`name: string`, `priority: int`, `callbackFunction: Function`) -> `null`
- **RegisterScriptAnalysisCallback**(`name: string`, `priority: int`, `callbackFunction: Function`) -> `null`
- **StripComments**(`code: string`) -> `string`
- **UpdateSourceAsync**(`script: LuaSourceContainer`, `callback: Function`) -> `null` [Yields]

## Events

- **TextDocumentDidChange**(`document: ScriptDocument`, `changesArray: Variant`)
- **TextDocumentDidClose**(`oldDocument: ScriptDocument`)
- **TextDocumentDidOpen**(`newDocument: ScriptDocument`)
