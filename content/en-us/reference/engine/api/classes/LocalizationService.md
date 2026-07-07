---
title: LocalizationService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# LocalizationService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **ForcePlayModeGameLocaleId**: `string` [Hidden] [NotReplicated] (Security: Read=LocalUserSecurity, Write=LocalUserSecurity)
- **ForcePlayModeRobloxLocaleId**: `string` [Hidden] [NotReplicated] (Security: Read=LocalUserSecurity, Write=LocalUserSecurity)
- **IsTextScraperRunning**: `bool` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **RobloxForcePlayModeGameLocaleId**: `string` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **RobloxForcePlayModeRobloxLocaleId**: `string` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **RobloxLocaleId**: `string` [ReadOnly] [NotReplicated]
- **SystemLocaleId**: `string` [ReadOnly] [NotReplicated]

## Methods

- **GetCorescriptLocalizations**() -> `Instances`
- **GetCountryRegionForPlayerAsync**(`player: Instance`) -> `string` [Yields]
- **GetIsLoadingInternalTranslations**() -> `bool`
- **GetTableEntries**(`instance: Instance = nil`) -> `Array`
- **GetTranslatorForLocaleAsync**(`locale: string`) -> `Instance` [Yields]
- **GetTranslatorForPlayer**(`player: Instance`) -> `Instance`
- **GetTranslatorForPlayerAsync**(`player: Instance`) -> `Instance` [Yields]
- **IsLoadingInternalTranslationsSettingChanged**(`newIsLoadingInternalTranslations: bool`) -> `null`
- **PromptDownloadGameTableToCSV**(`table: Instance`) -> `null` [Yields]
- **PromptExportToCSVs**() -> `null` [Yields]
- **PromptImportFromCSVs**() -> `null` [Yields]
- **PromptUploadCSVToGameTable**() -> `Instance` [Yields]
- **SetRobloxLocaleId**(`locale: string`) -> `null`
- **StartTextScraper**() -> `null`
- **StopTextScraper**() -> `null`

## Events

- **AutoTranslateWillRun**()
