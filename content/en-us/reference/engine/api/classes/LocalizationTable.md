---
title: LocalizationTable
type: class
superclass: Instance
---

# LocalizationTable

A LocalizationTable is a database of translations. It contains source strings
and translations for various languages.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

A LocalizationTable is a database of translations. It contains source strings
and translations for various languages. It is used with the `Class.Translator`
and `Class.LocalizationService` auto-translator system to control text
translations in the game. LocalizationTables are designed to be treated as
resources, like a texture or a script. They are not optimized to be modified
at runtime. Changing the contents of a table will cause the entire contents of
the table to be replicated to all players.

## LocalizationTable Entries

Each LocalizationTable contains a set of entries. Each entry contains the
translations of the text, along with some special fields:

- **Key** is an optional unique key for fast hash lookups in code. If it is
  non-empty it must be unique in the table.
- **Source** is the original text in the source language that will be used by
  the `Class.LocalizationService` automatic text replacement system to match
  GUI text and render a translation instead. The Source field can be filled by
  the text capture tools, or can be set manually. For key-based lookups the
  Source value can be used as a translation for
  `Class.LocalizationTable.SourceLocaleId` if the entry doesn't have a
  translation for that locale. If Source is empty then the entry will not be
  used by the automatic replacement system.
- **Context** is the full Instance name for the object that the text appeared
  on. Context is used for disambiguation by the automatic text replacement
  system. When multiple matches for the Source are found, the system will pick
  the best match by matching backwards from the end of the Context string.
  There are other more robust ways to handle disambiguation available as well,
  like using multiple tables with `Class.GuiBase2d.RootLocalizationTable`.
- **Example** is whatever you want it to be. If the text capture tool guessed
  some parameters for a string the Example field will contain an example of
  them used in context.

All of these fields are optional, but at least either Key or Source must be
non-empty. No two entries can have the same Key, Source, and Context.

See
[Translating Dynamic Content](../../../production/localization/translate-dynamic-content.md)
for more information.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.LocalizationTable.DevelopmentLanguage` | `string` | [Hidden] [NotReplicated] [Deprecated] |
| `Class.LocalizationTable.Root` | `Class.Instance` | [Hidden] [NotReplicated] [Deprecated] |
| `Class.LocalizationTable.SourceLocaleId` | `string` |  |

## Methods

### `Class.LocalizationTable:GetContents`

``GetContents()`` -> `string`
  [Deprecated]

### `Class.LocalizationTable:GetEntries`

``GetEntries()`` -> `Array`

### `Class.LocalizationTable:GetString`

``GetString(targetLocaleId: `string`, key: `string`)`` -> `string`
  [Deprecated]

### `Class.LocalizationTable:GetTranslator`

``GetTranslator(localeId: `string`)`` -> `Class.Instance`

### `Class.LocalizationTable:RemoveEntry`

``RemoveEntry(key: `string`, source: `string`, context: `string`)`` -> `null`

### `Class.LocalizationTable:RemoveEntryValue`

``RemoveEntryValue(key: `string`, source: `string`, context: `string`, localeId: `string`)`` -> `null`

### `Class.LocalizationTable:RemoveKey`

``RemoveKey(key: `string`)`` -> `null`
  [Deprecated]

### `Class.LocalizationTable:RemoveTargetLocale`

``RemoveTargetLocale(localeId: `string`)`` -> `null`

### `Class.LocalizationTable:SetContents`

``SetContents(contents: `string`)`` -> `null`
  [Deprecated]

### `Class.LocalizationTable:SetEntries`

``SetEntries(entries: `Variant`)`` -> `null`

### `Class.LocalizationTable:SetEntry`

``SetEntry(key: `string`, targetLocaleId: `string`, text: `string`)`` -> `null`
  [Deprecated]

### `Class.LocalizationTable:SetEntryContext`

``SetEntryContext(key: `string`, source: `string`, context: `string`, newContext: `string`)`` -> `null`

### `Class.LocalizationTable:SetEntryExample`

``SetEntryExample(key: `string`, source: `string`, context: `string`, example: `string`)`` -> `null`

### `Class.LocalizationTable:SetEntryKey`

``SetEntryKey(key: `string`, source: `string`, context: `string`, newKey: `string`)`` -> `null`

### `Class.LocalizationTable:SetEntrySource`

``SetEntrySource(key: `string`, source: `string`, context: `string`, newSource: `string`)`` -> `null`

### `Class.LocalizationTable:SetEntryValue`

``SetEntryValue(key: `string`, source: `string`, context: `string`, localeId: `string`, text: `string`)`` -> `null`

### `Class.LocalizationTable:SetIsExemptFromUGCAnalytics`

``SetIsExemptFromUGCAnalytics(value: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}
