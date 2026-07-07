---
title: LocalizationTable
type: class
superclass: Instance
---

# LocalizationTable

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.LocalizationTable.DevelopmentLanguage` | `string` | [Hidden] [NotReplicated] [Deprecated] |
| `Class.LocalizationTable.Root` | `Class.Instance` | [Hidden] [NotReplicated] [Deprecated] |
| `Class.LocalizationTable.SourceLocaleId` | `string` |  |

## Methods

### `Class.LocalizationTable:GetContents`

``GetContents()`` → `string`
  [Deprecated]

### `Class.LocalizationTable:GetEntries`

``GetEntries()`` → `Array`

### `Class.LocalizationTable:GetString`

``GetString(targetLocaleId: `string`, key: `string`)`` → `string`
  [Deprecated]

### `Class.LocalizationTable:GetTranslator`

``GetTranslator(localeId: `string`)`` → `Class.Instance`

### `Class.LocalizationTable:RemoveEntry`

``RemoveEntry(key: `string`, source: `string`, context: `string`)`` → `null`

### `Class.LocalizationTable:RemoveEntryValue`

``RemoveEntryValue(key: `string`, source: `string`, context: `string`, localeId: `string`)`` → `null`

### `Class.LocalizationTable:RemoveKey`

``RemoveKey(key: `string`)`` → `null`
  [Deprecated]

### `Class.LocalizationTable:RemoveTargetLocale`

``RemoveTargetLocale(localeId: `string`)`` → `null`

### `Class.LocalizationTable:SetContents`

``SetContents(contents: `string`)`` → `null`
  [Deprecated]

### `Class.LocalizationTable:SetEntries`

``SetEntries(entries: `Variant`)`` → `null`

### `Class.LocalizationTable:SetEntry`

``SetEntry(key: `string`, targetLocaleId: `string`, text: `string`)`` → `null`
  [Deprecated]

### `Class.LocalizationTable:SetEntryContext`

``SetEntryContext(key: `string`, source: `string`, context: `string`, newContext: `string`)`` → `null`

### `Class.LocalizationTable:SetEntryExample`

``SetEntryExample(key: `string`, source: `string`, context: `string`, example: `string`)`` → `null`

### `Class.LocalizationTable:SetEntryKey`

``SetEntryKey(key: `string`, source: `string`, context: `string`, newKey: `string`)`` → `null`

### `Class.LocalizationTable:SetEntrySource`

``SetEntrySource(key: `string`, source: `string`, context: `string`, newSource: `string`)`` → `null`

### `Class.LocalizationTable:SetEntryValue`

``SetEntryValue(key: `string`, source: `string`, context: `string`, localeId: `string`, text: `string`)`` → `null`

### `Class.LocalizationTable:SetIsExemptFromUGCAnalytics`

``SetIsExemptFromUGCAnalytics(value: `bool`)`` → `null`
   {security: RobloxScriptSecurity}
