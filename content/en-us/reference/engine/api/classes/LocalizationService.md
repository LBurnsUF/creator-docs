---
title: LocalizationService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# LocalizationService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.LocalizationService.ForcePlayModeGameLocaleId` | `string` | [Hidden] [NotReplicated] {security: LocalUserSecurity} |
| `Class.LocalizationService.ForcePlayModeRobloxLocaleId` | `string` | [Hidden] [NotReplicated] {security: LocalUserSecurity} |
| `Class.LocalizationService.IsTextScraperRunning` | `bool` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.LocalizationService.RobloxForcePlayModeGameLocaleId` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.LocalizationService.RobloxForcePlayModeRobloxLocaleId` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.LocalizationService.RobloxLocaleId` | `string` | [ReadOnly] [NotReplicated] |
| `Class.LocalizationService.SystemLocaleId` | `string` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.LocalizationService:GetCorescriptLocalizations`

``GetCorescriptLocalizations()`` → `Datatype.Instances`

### `Class.LocalizationService:GetCountryRegionForPlayerAsync`

``GetCountryRegionForPlayerAsync(player: `Class.Instance`)`` → `string`
  [Yields]

### `Class.LocalizationService:GetIsLoadingInternalTranslations`

``GetIsLoadingInternalTranslations()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.LocalizationService:GetTableEntries`

``GetTableEntries(instance: `Class.Instance`)`` → `Array`

### `Class.LocalizationService:GetTranslatorForLocaleAsync`

``GetTranslatorForLocaleAsync(locale: `string`)`` → `Class.Instance`
  [Yields]

### `Class.LocalizationService:GetTranslatorForPlayer`

``GetTranslatorForPlayer(player: `Class.Instance`)`` → `Class.Instance`

### `Class.LocalizationService:GetTranslatorForPlayerAsync`

``GetTranslatorForPlayerAsync(player: `Class.Instance`)`` → `Class.Instance`
  [Yields]

### `Class.LocalizationService:IsLoadingInternalTranslationsSettingChanged`

``IsLoadingInternalTranslationsSettingChanged(newIsLoadingInternalTranslations: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.LocalizationService:PromptDownloadGameTableToCSV`

``PromptDownloadGameTableToCSV(table: `Class.Instance`)`` → `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.LocalizationService:PromptExportToCSVs`

``PromptExportToCSVs()`` → `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.LocalizationService:PromptImportFromCSVs`

``PromptImportFromCSVs()`` → `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.LocalizationService:PromptUploadCSVToGameTable`

``PromptUploadCSVToGameTable()`` → `Class.Instance`
  [Yields] {security: RobloxScriptSecurity}

### `Class.LocalizationService:SetRobloxLocaleId`

``SetRobloxLocaleId(locale: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.LocalizationService:StartTextScraper`

``StartTextScraper()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.LocalizationService:StopTextScraper`

``StopTextScraper()`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.LocalizationService.AutoTranslateWillRun`

Fires with: ()
