---
title: BaseImportData
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# BaseImportData

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.BaseImportData.Id` | `string` | [ReadOnly] [NotReplicated] |
| `Class.BaseImportData.ImportName` | `string` |  |
| `Class.BaseImportData.ShouldImport` | `bool` |  |

## Methods

### `Class.BaseImportData:CreatePresetFromData`

``CreatePresetFromData()`` -> `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.BaseImportData:GetPreview`

``GetPreview()`` -> `Class.Instance`
   {security: RobloxScriptSecurity}

### `Class.BaseImportData:GetStatuses`

``GetStatuses()`` -> `Dictionary`
   {security: RobloxScriptSecurity}

## Events

### `Class.BaseImportData.StatusRemoved`

Fires with: (status: `Dictionary`)

### `Class.BaseImportData.StatusReported`

Fires with: (status: `Dictionary`)
