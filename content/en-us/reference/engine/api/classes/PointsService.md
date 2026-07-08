---
title: PointsService
type: class
superclass: Instance
tags: [NotCreatable, Service, Deprecated]
---

# PointsService

This service controls the points award system used to showcase a player's
achievements and participation throughout Roblox.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [Deprecated]

## Description

The PointsService class controls points.

Points are an award system used to showcase a player's achievements and
participation throughout Roblox. How points are awarded through this service
is at the discretion of the game's developer.

> **Deprecated:** This class was once used to control an ancient achievement system since
removed and deprecated. It and its members should not be used in new work.

## Methods

### `Class.PointsService:AwardPoints`

``AwardPoints(userId: `int64`, amount: `int`)`` -> `Tuple`
  [Yields] [Deprecated]

### `Class.PointsService:GetAwardablePoints`

``GetAwardablePoints()`` -> `int`
  [Deprecated]

### `Class.PointsService:GetGamePointBalance`

``GetGamePointBalance(userId: `int64`)`` -> `int`
  [Yields] [Deprecated]

### `Class.PointsService:GetPointBalance`

``GetPointBalance(userId: `int64`)`` -> `int`
  [Yields] [Deprecated]

## Events

### `Class.PointsService.PointsAwarded`

Fires with: (userId: `int64`, pointsAwarded: `int`, userBalanceInGame: `int`, userTotalBalance: `int`)
