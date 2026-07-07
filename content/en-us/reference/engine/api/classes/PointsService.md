---
title: PointsService
type: class
superclass: Instance
tags: [NotCreatable, Service, Deprecated]
---

# PointsService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [Deprecated]

## Methods

### `Class.PointsService:AwardPoints`

``AwardPoints(userId: `int64`, amount: `int`)`` → `Tuple`
  [Yields] [Deprecated]

### `Class.PointsService:GetAwardablePoints`

``GetAwardablePoints()`` → `int`
  [Deprecated]

### `Class.PointsService:GetGamePointBalance`

``GetGamePointBalance(userId: `int64`)`` → `int`
  [Yields] [Deprecated]

### `Class.PointsService:GetPointBalance`

``GetPointBalance(userId: `int64`)`` → `int`
  [Yields] [Deprecated]

## Events

### `Class.PointsService.PointsAwarded`

Fires with: (userId: `int64`, pointsAwarded: `int`, userBalanceInGame: `int`, userTotalBalance: `int`)
