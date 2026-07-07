---
title: ScriptDocument
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# ScriptDocument

**Inherits**: Instance > Object

**Tags**: NotCreatable, NotReplicated

## Methods

- **CloseAsync**() -> `Tuple` [Yields]
- **EditTextAsync**(`newText: string`, `startLine: int`, `startCharacter: int`, `endLine: int`, `endCharacter: int`) -> `Tuple` [Yields]
- **ForceSetSelectionAsync**(`cursorLine: int`, `cursorCharacter: int`, `anchorLine: int? = nil`, `anchorCharacter: int? = nil`) -> `Tuple` [Yields]
- **GetInternalUri**() -> `string`
- **GetLine**(`lineIndex: int? = nil`) -> `string`
- **GetLineCount**() -> `int`
- **GetScript**() -> `LuaSourceContainer`
- **GetSelectedText**() -> `string`
- **GetSelection**() -> `Tuple`
- **GetSelectionEnd**() -> `Tuple`
- **GetSelectionStart**() -> `Tuple`
- **GetText**(`startLine: int? = nil`, `startCharacter: int? = nil`, `endLine: int? = nil`, `endCharacter: int? = nil`) -> `string`
- **GetViewport**() -> `Tuple`
- **HasSelectedText**() -> `bool`
- **IsCommandBar**() -> `bool`
- **MultiEditTextAsync**(`edits: Array`) -> `Tuple` [Yields]
- **RequestSetSelectionAsync**(`cursorLine: int`, `cursorCharacter: int`, `anchorLine: int? = nil`, `anchorCharacter: int? = nil`) -> `Tuple` [Yields]

## Events

- **SelectionChanged**(`positionLine: int64`, `positionCharacter: int64`, `anchorLine: int64`, `anchorCharacter: int64`)
- **ViewportChanged**(`startLine: int64`, `endLine: int64`)
