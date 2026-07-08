---
title: ScriptDocument
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# ScriptDocument

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

A `Class.ScriptDocument` instance is a proxy of the document of a Studio
Script Editor. It's different from the `Class.LuaSourceContainer` open in the
editor in that it represents the ephemeral state of an open document, and its
representation is in a format that's more suited for reading and editing code
than executing it. In particular, `Class.ScriptDocument` reflects any changes
that have been made to the open script in Drafts Mode, which the source
property doesn't.

The Script Editor itself exists and changes on a different thread than any
`Class.DataModel`, so the `Class.ScriptDocument` replicates the open Script
Editor, but it isn't the open editor. Because of the replication, there's
sometimes a slight delay between changing the text in the editor and updating
the `Class.ScriptDocument`. The delay usually occurs because the
`Class.DataModel` is busy, and it's almost always extremely small, but it
still exists.

The existence of a `Class.ScriptDocument` indicates that a document is open in
the Script Editor. All `Class.ScriptDocument` instances have
`Class.ScriptEditorService` as its parent. Each instance adheres to the
following encoding conventions:

- All text in `Class.ScriptDocument` is UTF-8 encoded.
- All line indices are 1-indexed.
- All character indices are 1-indexed and count UTF-8 bytes, not graphemes, so
  the same warning from `Class.TextBox.CursorPosition` applies: many Unicode
  characters take more than one byte.
- All ranges are inclusive of their start position and exclusive of their end
  position, so start == end implies an empty range.

All APIs for `Class.ScriptDocument` are at **Plugin** level security.

## Methods

### `Class.ScriptDocument:CloseAsync`

``CloseAsync()`` -> `Tuple`
  [Yields] {security: PluginSecurity}

### `Class.ScriptDocument:EditTextAsync`

``EditTextAsync(newText: `string`, startLine: `int`, startCharacter: `int`, endLine: `int`, endCharacter: `int`)`` -> `Tuple`
  [Yields] {security: PluginSecurity}

### `Class.ScriptDocument:ForceSetSelectionAsync`

``ForceSetSelectionAsync(cursorLine: `int`, cursorCharacter: `int`, anchorLine: `int?`, anchorCharacter: `int?`)`` -> `Tuple`
  [Yields] {security: PluginSecurity}

### `Class.ScriptDocument:GetInternalUri`

``GetInternalUri()`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.ScriptDocument:GetLine`

``GetLine(lineIndex: `int?`)`` -> `string`
   {security: PluginSecurity}

### `Class.ScriptDocument:GetLineCount`

``GetLineCount()`` -> `int`
   {security: PluginSecurity}

### `Class.ScriptDocument:GetScript`

``GetScript()`` -> `Class.LuaSourceContainer`
   {security: PluginSecurity}

### `Class.ScriptDocument:GetSelectedText`

``GetSelectedText()`` -> `string`
   {security: PluginSecurity}

### `Class.ScriptDocument:GetSelection`

``GetSelection()`` -> `Tuple`
   {security: PluginSecurity}

### `Class.ScriptDocument:GetSelectionEnd`

``GetSelectionEnd()`` -> `Tuple`
   {security: PluginSecurity}

### `Class.ScriptDocument:GetSelectionStart`

``GetSelectionStart()`` -> `Tuple`
   {security: PluginSecurity}

### `Class.ScriptDocument:GetText`

``GetText(startLine: `int?`, startCharacter: `int?`, endLine: `int?`, endCharacter: `int?`)`` -> `string`
   {security: PluginSecurity}

### `Class.ScriptDocument:GetViewport`

``GetViewport()`` -> `Tuple`
   {security: PluginSecurity}

### `Class.ScriptDocument:HasSelectedText`

``HasSelectedText()`` -> `bool`
   {security: PluginSecurity}

### `Class.ScriptDocument:IsCommandBar`

``IsCommandBar()`` -> `bool`
   {security: PluginSecurity}

### `Class.ScriptDocument:MultiEditTextAsync`

``MultiEditTextAsync(edits: `Array`)`` -> `Tuple`
  [Yields] {security: PluginSecurity}

### `Class.ScriptDocument:RequestSetSelectionAsync`

``RequestSetSelectionAsync(cursorLine: `int`, cursorCharacter: `int`, anchorLine: `int?`, anchorCharacter: `int?`)`` -> `Tuple`
  [Yields] {security: PluginSecurity}

## Events

### `Class.ScriptDocument.SelectionChanged`

Fires with: (positionLine: `int64`, positionCharacter: `int64`, anchorLine: `int64`, anchorCharacter: `int64`)

### `Class.ScriptDocument.ViewportChanged`

Fires with: (startLine: `int64`, endLine: `int64`)
