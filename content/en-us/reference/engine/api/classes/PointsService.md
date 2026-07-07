---
title: PointsService
type: class
superclass: Instance
tags: [NotCreatable, Service, Deprecated]
---

# PointsService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, Deprecated

## Methods

- **AwardPoints**(`userId: int64`, `amount: int`) -> `Tuple` [Yields] [Deprecated]
- **GetAwardablePoints**() -> `int` [Deprecated]
- **GetGamePointBalance**(`userId: int64`) -> `int` [Yields] [Deprecated]
- **GetPointBalance**(`userId: int64`) -> `int` [Yields] [Deprecated]

## Events

- **PointsAwarded**(`userId: int64`, `pointsAwarded: int`, `userBalanceInGame: int`, `userTotalBalance: int`)
