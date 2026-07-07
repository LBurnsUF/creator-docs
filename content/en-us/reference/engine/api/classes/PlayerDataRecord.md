---
title: PlayerDataRecord
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# PlayerDataRecord

**Inherits**: Instance > Object

**Tags**: NotCreatable, NotReplicated

## Properties

- **CreatedTime**: `int64` [ReadOnly] [NotReplicated]
- **DefaultRecordName**: `bool` [ReadOnly] [NotReplicated]
- **Dirty**: `bool` [ReadOnly] [NotReplicated]
- **Error**: `PlayerDataErrorState` [ReadOnly] [NotReplicated]
- **FlushedTime**: `int64` [ReadOnly] [NotReplicated]
- **LoadedTime**: `int64` [ReadOnly] [NotReplicated]
- **ModifiedTime**: `int64` [ReadOnly] [NotReplicated]
- **NewRecord**: `bool` [ReadOnly] [NotReplicated]
- **Readable**: `bool` [ReadOnly] [NotReplicated]
- **RecordName**: `string` [ReadOnly] [NotReplicated]
- **Writable**: `bool` [ReadOnly] [NotReplicated]

## Methods

- **GetPlayer**() -> `Player`
- **GetValue**(`key: string`) -> `Variant`
- **GetValueChangedSignal**(`key: string`) -> `RBXScriptSignal`
- **ReleaseAsync**() -> `null` [Yields]
- **RemoveValue**(`key: string`) -> `null`
- **RequestFlushAsync**() -> `null` [Yields]
- **SetValue**(`key: string`, `value: Variant`) -> `null`

## Events

- **Changed**(`key: string`, `value: Variant`)
- **Flushed**(`flushState: bool`, `error: string?`)
- **Loaded**(`success: bool`, `error: string?`)
