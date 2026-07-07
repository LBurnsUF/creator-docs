---
title: GlobalDataStore
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# GlobalDataStore

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Methods

### `Class.GlobalDataStore:GetAsync`

``GetAsync(key: `string`, options: `Class.DataStoreGetOptions`)`` → `Tuple`
  [Yields]

### `Class.GlobalDataStore:IncrementAsync`

``IncrementAsync(key: `string`, delta: `int`, userIds: `Array`, options: `Class.DataStoreIncrementOptions`)`` → `Variant`
  [Yields]

### `Class.GlobalDataStore:OnUpdate`

``OnUpdate(key: `string`, callback: `Datatype.Function`)`` → `Datatype.RBXScriptConnection`
  [Deprecated]

### `Class.GlobalDataStore:RemoveAsync`

``RemoveAsync(key: `string`)`` → `Tuple`
  [Yields]

### `Class.GlobalDataStore:SetAsync`

``SetAsync(key: `string`, value: `Variant`, userIds: `Array`, options: `Class.DataStoreSetOptions`)`` → `Variant`
  [Yields]

### `Class.GlobalDataStore:UpdateAsync`

``UpdateAsync(key: `string`, transformFunction: `Datatype.Function`)`` → `Tuple`
  [Yields]
