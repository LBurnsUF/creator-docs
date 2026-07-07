---
title: ScriptDocument
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# ScriptDocument

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Methods

### `Class.ScriptDocument:CloseAsync`

``CloseAsync()`` → `Tuple`
  [Yields] {security: PluginSecurity}

### `Class.ScriptDocument:EditTextAsync`

``EditTextAsync(newText: `string`, startLine: `int`, startCharacter: `int`, endLine: `int`, endCharacter: `int`)`` → `Tuple`
  [Yields] {security: PluginSecurity}

### `Class.ScriptDocument:ForceSetSelectionAsync`

``ForceSetSelectionAsync(cursorLine: `int`, cursorCharacter: `int`, anchorLine: `int?`, anchorCharacter: `int?`)`` → `Tuple`
  [Yields] {security: PluginSecurity}

### `Class.ScriptDocument:GetInternalUri`

``GetInternalUri()`` → `string`
   {security: RobloxScriptSecurity}

### `Class.ScriptDocument:GetLine`

``GetLine(lineIndex: `int?`)`` → `string`
   {security: PluginSecurity}

### `Class.ScriptDocument:GetLineCount`

``GetLineCount()`` → `int`
   {security: PluginSecurity}

### `Class.ScriptDocument:GetScript`

``GetScript()`` → `Class.LuaSourceContainer`
   {security: PluginSecurity}

### `Class.ScriptDocument:GetSelectedText`

``GetSelectedText()`` → `string`
   {security: PluginSecurity}

### `Class.ScriptDocument:GetSelection`

``GetSelection()`` → `Tuple`
   {security: PluginSecurity}

### `Class.ScriptDocument:GetSelectionEnd`

``GetSelectionEnd()`` → `Tuple`
   {security: PluginSecurity}

### `Class.ScriptDocument:GetSelectionStart`

``GetSelectionStart()`` → `Tuple`
   {security: PluginSecurity}

### `Class.ScriptDocument:GetText`

``GetText(startLine: `int?`, startCharacter: `int?`, endLine: `int?`, endCharacter: `int?`)`` → `string`
   {security: PluginSecurity}

### `Class.ScriptDocument:GetViewport`

``GetViewport()`` → `Tuple`
   {security: PluginSecurity}

### `Class.ScriptDocument:HasSelectedText`

``HasSelectedText()`` → `bool`
   {security: PluginSecurity}

### `Class.ScriptDocument:IsCommandBar`

``IsCommandBar()`` → `bool`
   {security: PluginSecurity}

### `Class.ScriptDocument:MultiEditTextAsync`

``MultiEditTextAsync(edits: `Array`)`` → `Tuple`
  [Yields] {security: PluginSecurity}

### `Class.ScriptDocument:RequestSetSelectionAsync`

``RequestSetSelectionAsync(cursorLine: `int`, cursorCharacter: `int`, anchorLine: `int?`, anchorCharacter: `int?`)`` → `Tuple`
  [Yields] {security: PluginSecurity}

## Events

### `Class.ScriptDocument.SelectionChanged`

Fires with: (positionLine: `int64`, positionCharacter: `int64`, anchorLine: `int64`, anchorCharacter: `int64`)

### `Class.ScriptDocument.ViewportChanged`

Fires with: (startLine: `int64`, endLine: `int64`)
