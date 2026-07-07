---
title: DataStoreService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# DataStoreService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **AutomaticRetry**: `bool` [NotReplicated] (Security: Read=LocalUserSecurity, Write=LocalUserSecurity)
- **LegacyNamingScheme**: `bool` [Hidden] [Deprecated] (Security: Read=LocalUserSecurity, Write=LocalUserSecurity)

## Methods

- **GetDataStore**(`name: string`, `scope: string = global`, `options: Instance = nil`) -> `DataStore`
- **GetGlobalDataStore**() -> `DataStore`
- **GetOrderedDataStore**(`name: string`, `scope: string = global`) -> `OrderedDataStore`
- **GetRequestBudgetForRequestType**(`requestType: DataStoreRequestType`) -> `int`
- **ListDataStoresAsync**(`prefix: string = `, `pageSize: int = 0`, `cursor: string = `) -> `DataStoreListingPages` [Yields]
- **SetRateLimitForRequestType**(`requestType: DataStoreRequestType`, `baseLimit: int`, `perPlayerLimit: int`) -> `null`
