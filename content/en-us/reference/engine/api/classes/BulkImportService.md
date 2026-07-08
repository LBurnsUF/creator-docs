---
title: BulkImportService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# BulkImportService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.BulkImportService:LaunchBulkImport`

``LaunchBulkImport(assetTypeToImport: `int`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.BulkImportService:ShowBulkImportView`

``ShowBulkImportView()`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.BulkImportService.AssetImported`

Fires with: (assetType: `Enum.AssetType`, name: `string`, id: `int64`)

### `Class.BulkImportService.BulkImportFinished`

Fires with: (state: `int`)

### `Class.BulkImportService.BulkImportStarted`

Fires with: ()
