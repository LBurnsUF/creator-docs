---
title: LocalizationTable
type: class
superclass: Instance
---

# LocalizationTable

**Inherits**: Instance > Object

## Properties

- **DevelopmentLanguage**: `string` [Hidden] [NotReplicated] [Deprecated]
- **Root**: `Instance` [Hidden] [NotReplicated] [Deprecated]
- **SourceLocaleId**: `string`

## Methods

- **GetContents**() -> `string` [Deprecated]
- **GetEntries**() -> `Array`
- **GetString**(`targetLocaleId: string`, `key: string`) -> `string` [Deprecated]
- **GetTranslator**(`localeId: string`) -> `Instance`
- **RemoveEntry**(`key: string`, `source: string`, `context: string`) -> `null`
- **RemoveEntryValue**(`key: string`, `source: string`, `context: string`, `localeId: string`) -> `null`
- **RemoveKey**(`key: string`) -> `null` [Deprecated]
- **RemoveTargetLocale**(`localeId: string`) -> `null`
- **SetContents**(`contents: string`) -> `null` [Deprecated]
- **SetEntries**(`entries: Variant`) -> `null`
- **SetEntry**(`key: string`, `targetLocaleId: string`, `text: string`) -> `null` [Deprecated]
- **SetEntryContext**(`key: string`, `source: string`, `context: string`, `newContext: string`) -> `null`
- **SetEntryExample**(`key: string`, `source: string`, `context: string`, `example: string`) -> `null`
- **SetEntryKey**(`key: string`, `source: string`, `context: string`, `newKey: string`) -> `null`
- **SetEntrySource**(`key: string`, `source: string`, `context: string`, `newSource: string`) -> `null`
- **SetEntryValue**(`key: string`, `source: string`, `context: string`, `localeId: string`, `text: string`) -> `null`
- **SetIsExemptFromUGCAnalytics**(`value: bool`) -> `null`
