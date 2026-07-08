---
title: PlayerDataRecord
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# PlayerDataRecord

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.PlayerDataRecord.CreatedTime` | `int64` | [ReadOnly] [NotReplicated] |
| `Class.PlayerDataRecord.DefaultRecordName` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.PlayerDataRecord.Dirty` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.PlayerDataRecord.Error` | `Enum.PlayerDataErrorState` | [ReadOnly] [NotReplicated] |
| `Class.PlayerDataRecord.FlushedTime` | `int64` | [ReadOnly] [NotReplicated] |
| `Class.PlayerDataRecord.LoadedTime` | `int64` | [ReadOnly] [NotReplicated] |
| `Class.PlayerDataRecord.ModifiedTime` | `int64` | [ReadOnly] [NotReplicated] |
| `Class.PlayerDataRecord.NewRecord` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.PlayerDataRecord.Readable` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.PlayerDataRecord.RecordName` | `string` | [ReadOnly] [NotReplicated] |
| `Class.PlayerDataRecord.Writable` | `bool` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.PlayerDataRecord:GetPlayer`

``GetPlayer()`` -> `Class.Player`

### `Class.PlayerDataRecord:GetValue`

``GetValue(key: `string`)`` -> `Variant`

### `Class.PlayerDataRecord:GetValueChangedSignal`

``GetValueChangedSignal(key: `string`)`` -> `Datatype.RBXScriptSignal`

### `Class.PlayerDataRecord:ReleaseAsync`

``ReleaseAsync()`` -> `null`
  [Yields]

### `Class.PlayerDataRecord:RemoveValue`

``RemoveValue(key: `string`)`` -> `null`

### `Class.PlayerDataRecord:RequestFlushAsync`

``RequestFlushAsync()`` -> `null`
  [Yields]

### `Class.PlayerDataRecord:SetValue`

``SetValue(key: `string`, value: `Variant`)`` -> `null`

## Events

### `Class.PlayerDataRecord.Changed`

Fires with: (key: `string`, value: `Variant`)

### `Class.PlayerDataRecord.Flushed`

Fires with: (flushState: `bool`, error: `string?`)

### `Class.PlayerDataRecord.Loaded`

Fires with: (success: `bool`, error: `string?`)
