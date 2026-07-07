---
title: BadgeService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# BadgeService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.BadgeService:AwardBadge`

``AwardBadge(userId: `Datatype.User`, badgeId: `int64`)`` → `bool`
  [Yields] [Deprecated]

### `Class.BadgeService:AwardBadgeAsync`

``AwardBadgeAsync(userId: `Datatype.User`, badgeId: `int64`)`` → `bool`
  [Yields]

### `Class.BadgeService:CheckUserBadgesAsync`

``CheckUserBadgesAsync(userId: `Datatype.User`, badgeIds: `Array`)`` → `Array`
  [Yields]

### `Class.BadgeService:GetBadgeInfoAsync`

``GetBadgeInfoAsync(badgeId: `int64`)`` → `Dictionary`
  [Yields]

### `Class.BadgeService:IsDisabled`

``IsDisabled(badgeId: `int64`)`` → `bool`
  [Yields] [Deprecated]

### `Class.BadgeService:IsLegal`

``IsLegal(badgeId: `int64`)`` → `bool`
  [Yields] [Deprecated]

### `Class.BadgeService:UserHasBadge`

``UserHasBadge(userId: `Datatype.User`, badgeId: `int64`)`` → `bool`
  [Yields] [Deprecated]

### `Class.BadgeService:UserHasBadgeAsync`

``UserHasBadgeAsync(userId: `Datatype.User`, badgeId: `int64`)`` → `bool`
  [Yields]

## Events

### `Class.BadgeService.BadgeAwarded`

Fires with: (message: `string`, userId: `int64`, badgeId: `int64`)

### `Class.BadgeService.OnBadgeAwarded`

Fires with: (userId: `int64`, creatorId: `int64`, badgeId: `int64`)
