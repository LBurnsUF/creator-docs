---
title: BulkImportService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# BulkImportService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **LaunchBulkImport**(`assetTypeToImport: int`) -> `null`
- **ShowBulkImportView**() -> `null`

## Events

- **AssetImported**(`assetType: AssetType`, `name: string`, `id: int64`)
- **BulkImportFinished**(`state: int`)
- **BulkImportStarted**()
