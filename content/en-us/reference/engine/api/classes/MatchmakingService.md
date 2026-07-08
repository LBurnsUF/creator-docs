---
title: MatchmakingService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# MatchmakingService

The service responsible for managing custom matchmaking data.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

`Class.MatchmakingService` is responsible for managing custom matchmaking
attributes. Use it to read and write matchmaking data.

## Methods

### `Class.MatchmakingService:GetServerAttribute`

``GetServerAttribute(name: `string`)`` -> `Tuple`

### `Class.MatchmakingService:InitializeServerAttributesForStudio`

``InitializeServerAttributesForStudio(serverAttributes: `Dictionary`)`` -> `Tuple`

### `Class.MatchmakingService:SetServerAttribute`

``SetServerAttribute(name: `string`, value: `Variant`)`` -> `Tuple`
