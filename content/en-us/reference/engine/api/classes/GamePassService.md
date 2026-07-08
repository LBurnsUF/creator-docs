---
title: GamePassService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# GamePassService

A service associated with the legacy game pass system. Use
`Class.MarketplaceService` for all new work.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

The GamePassService is a service that supports legacy game passes using _Asset
IDs_. `Class.MarketplaceService` should be used for all new game passes.

For more information about game passes, please see
[Game Passes](../../../production/monetization/passes.md).

## Methods

### `Class.GamePassService:PlayerHasPass`

``PlayerHasPass(player: `Class.Player`, gamePassId: `int64`)`` -> `bool`
  [Yields] [Deprecated]
