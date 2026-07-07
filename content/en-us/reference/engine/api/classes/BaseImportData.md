---
title: BaseImportData
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# BaseImportData

**Inherits**: Instance > Object

**Tags**: NotCreatable, NotReplicated

## Properties

- **Id**: `string` [ReadOnly] [NotReplicated]
- **ImportName**: `string`
- **ShouldImport**: `bool`

## Methods

- **CreatePresetFromData**() -> `Dictionary`
- **GetPreview**() -> `Instance`
- **GetStatuses**() -> `Dictionary`

## Events

- **StatusRemoved**(`status: Dictionary`)
- **StatusReported**(`status: Dictionary`)
