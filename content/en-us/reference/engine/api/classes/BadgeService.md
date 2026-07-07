---
title: BadgeService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# BadgeService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **AwardBadge**(`userId: User`, `badgeId: int64`) -> `bool` [Yields] [Deprecated]
- **AwardBadgeAsync**(`userId: User`, `badgeId: int64`) -> `bool` [Yields]
- **CheckUserBadgesAsync**(`userId: User`, `badgeIds: Array`) -> `Array` [Yields]
- **GetBadgeInfoAsync**(`badgeId: int64`) -> `Dictionary` [Yields]
- **IsDisabled**(`badgeId: int64`) -> `bool` [Yields] [Deprecated]
- **IsLegal**(`badgeId: int64`) -> `bool` [Yields] [Deprecated]
- **UserHasBadge**(`userId: User`, `badgeId: int64`) -> `bool` [Yields] [Deprecated]
- **UserHasBadgeAsync**(`userId: User`, `badgeId: int64`) -> `bool` [Yields]

## Events

- **BadgeAwarded**(`message: string`, `userId: int64`, `badgeId: int64`)
- **OnBadgeAwarded**(`userId: int64`, `creatorId: int64`, `badgeId: int64`)
