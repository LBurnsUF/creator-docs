---
title: DataStoreService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# DataStoreService

A game service that gives access to persistent data storage across places in a
game.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

**DataStoreService** exposes methods for getting `Class.GlobalDataStore` and
`Class.OrderedDataStore` objects. Data stores can only be accessed by game
servers, so you can only use `Class.DataStoreService` within a `Class.Script`
or a `Class.ModuleScript` that is used by a `Class.Script`.

See [Data stores](../../../cloud-services/data-stores/index.md) for an
in-depth guide on data structure, management, error handling, limits, and
more.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.DataStoreService.AutomaticRetry` | `bool` | [NotReplicated] {security: LocalUserSecurity} |
| `Class.DataStoreService.LegacyNamingScheme` | `bool` | [Hidden] [Deprecated] {security: LocalUserSecurity} |

## Methods

### `Class.DataStoreService:GetDataStore`

``GetDataStore(name: `string`, scope: `string`, options: `Class.Instance`)`` -> `Class.DataStore`

### `Class.DataStoreService:GetGlobalDataStore`

``GetGlobalDataStore()`` -> `Class.DataStore`

### `Class.DataStoreService:GetOrderedDataStore`

``GetOrderedDataStore(name: `string`, scope: `string`)`` -> `Class.OrderedDataStore`

### `Class.DataStoreService:GetRequestBudgetForRequestType`

``GetRequestBudgetForRequestType(requestType: `Enum.DataStoreRequestType`)`` -> `int`

### `Class.DataStoreService:ListDataStoresAsync`

``ListDataStoresAsync(prefix: `string`, pageSize: `int`, cursor: `string`)`` -> `Class.DataStoreListingPages`
  [Yields]

### `Class.DataStoreService:SetRateLimitForRequestType`

``SetRateLimitForRequestType(requestType: `Enum.DataStoreRequestType`, baseLimit: `int`, perPlayerLimit: `int`)`` -> `null`
