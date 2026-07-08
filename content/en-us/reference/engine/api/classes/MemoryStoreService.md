---
title: MemoryStoreService
type: class
superclass: Instance
tags: [Service]
---

# MemoryStoreService

Exposes methods to access specific primitives within MemoryStore.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [Service]

## Description

A top-level singleton class which exposes methods to access specific
primitives within the MemoryStoreService. Use it for any data that rapidly
changes that other servers can restore, such as global leaderboards,
matchmaking queues, and auction houses.

For a more in-depth look, see
[Memory Stores](../../../cloud-services/memory-stores/index.md). For the
limits and quotas of the service, see
[Limits and Quotas](../../../cloud-services/memory-stores/index.md#limits-and-quotas).

## Methods

### `Class.MemoryStoreService:GetHashMap`

``GetHashMap(name: `string`)`` -> `Class.MemoryStoreHashMap`

### `Class.MemoryStoreService:GetQueue`

``GetQueue(name: `string`, invisibilityTimeout: `int`)`` -> `Class.MemoryStoreQueue`

### `Class.MemoryStoreService:GetSortedMap`

``GetSortedMap(name: `string`)`` -> `Class.MemoryStoreSortedMap`
