---
title: DataStoreRequestType
type: enum
---

# `Enum.DataStoreRequestType`

Indicates the type of data store request being made.

Indicates the type of data store request being made.

The `Enum.DataStoreRequestType` enum has 17 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.DataStoreRequestType.GetAsync` | 0 | Refers to `Class.GlobalDataStore:GetAsync()/GetAsync()` and the read of `Class.GlobalDataStore:Updat |
| `Enum.DataStoreRequestType.SetIncrementAsync` | 1 | Refers to `Class.DataStore:SetAsync()/SetAsync()`, `Class.DataStore:IncrementAsync()/IncrementAsync( |
| `Enum.DataStoreRequestType.UpdateAsync` | 2 | Refers to `Class.GlobalDataStore:UpdateAsync()/UpdateAsync()`. |
| `Enum.DataStoreRequestType.GetSortedAsync` | 3 | Refers to `Class.OrderedDataStore:GetSortedAsync()/GetSortedAsync()`. |
| `Enum.DataStoreRequestType.SetIncrementSortedAsync` | 4 | Refers to `Class.OrderedDataStore:SetAsync()/SetAsync()` `Class.OrderedDataStore:IncrementAsync()/In |
| `Enum.DataStoreRequestType.OnUpdate` | 5 | Refers to `Class.GlobalDataStore:OnUpdate()/OnUpdate()`. |
| `Enum.DataStoreRequestType.ListAsync` | 6 | Refers to `Class.DataStore:ListKeysAsync()/ListKeysAsync()` and `Class.DataStore:ListVersionsAsync() |
| `Enum.DataStoreRequestType.GetVersionAsync` | 7 | Refers to `Class.DataStore:GetVersionAsync()/GetVersionAsync()`. |
| `Enum.DataStoreRequestType.RemoveVersionAsync` | 8 | Refers to `Class.DataStore:RemoveVersionAsync()/RemoveVersionAsync()`. |
| `Enum.DataStoreRequestType.StandardRead` | 9 | Refers to `Class.DataStore:GetAsync()/GetAsync()`, `Class.DataStore:GetVersionAsync()/GetVersionAsyn |
| `Enum.DataStoreRequestType.StandardWrite` | 10 | Refers to `Class.DataStore:SetAsync()/SetAsync()`, `Class.DataStore:IncrementAsync()/IncrementAsync( |
| `Enum.DataStoreRequestType.StandardList` | 11 | Refers to `Class.DataStoreService:ListDataStoresAsync()/ListDataStoresAsync()`, and `Class.DataStore |
| `Enum.DataStoreRequestType.StandardRemove` | 12 | Refers to `Class.DataStore:RemoveAsync()/RemoveAsync()` for `Class.DataStore/DataStore`. |
| `Enum.DataStoreRequestType.OrderedRead` | 13 | Refers to `Class.OrderedDataStore:GetAsync()/GetAsync()` and the read of `Class.OrderedDataStore:Upd |
| `Enum.DataStoreRequestType.OrderedWrite` | 14 | Refers to `Class.OrderedDataStore:SetAsync()/SetAsync()`, `Class.OrderedDataStore:IncrementAsync()/I |
| `Enum.DataStoreRequestType.OrderedList` | 15 | Refers to `Class.OrderedDataStore:GetSortedAsync()/GetSortedAsync()` for `Class.OrderedDataStore/Ord |
| `Enum.DataStoreRequestType.OrderedRemove` | 16 | Refers to `Class.OrderedDataStore:RemoveAsync()/RemoveAsync()` for `Class.OrderedDataStore/OrderedDa |
