---
title: DataStoreService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# DataStoreService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.DataStoreService.AutomaticRetry` | `bool` | [NotReplicated] {security: LocalUserSecurity} |
| `Class.DataStoreService.LegacyNamingScheme` | `bool` | [Hidden] [Deprecated] {security: LocalUserSecurity} |

## Methods

### `Class.DataStoreService:GetDataStore`

``GetDataStore(name: `string`, scope: `string`, options: `Class.Instance`)`` → `Class.DataStore`

### `Class.DataStoreService:GetGlobalDataStore`

``GetGlobalDataStore()`` → `Class.DataStore`

### `Class.DataStoreService:GetOrderedDataStore`

``GetOrderedDataStore(name: `string`, scope: `string`)`` → `Class.OrderedDataStore`

### `Class.DataStoreService:GetRequestBudgetForRequestType`

``GetRequestBudgetForRequestType(requestType: `Enum.DataStoreRequestType`)`` → `int`

### `Class.DataStoreService:ListDataStoresAsync`

``ListDataStoresAsync(prefix: `string`, pageSize: `int`, cursor: `string`)`` → `Class.DataStoreListingPages`
  [Yields]

### `Class.DataStoreService:SetRateLimitForRequestType`

``SetRateLimitForRequestType(requestType: `Enum.DataStoreRequestType`, baseLimit: `int`, perPlayerLimit: `int`)`` → `null`
