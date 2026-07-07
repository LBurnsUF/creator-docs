---
title: PhysicsService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# PhysicsService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.PhysicsService:CollisionGroupContainsPart`

``CollisionGroupContainsPart(name: `string`, part: `Class.BasePart`)`` → `bool`
  [Deprecated]

### `Class.PhysicsService:CollisionGroupSetCollidable`

``CollisionGroupSetCollidable(name1: `string`, name2: `string`, collidable: `bool`)`` → `null`

### `Class.PhysicsService:CollisionGroupsAreCollidable`

``CollisionGroupsAreCollidable(name1: `string`, name2: `string`)`` → `bool`

### `Class.PhysicsService:CreateCollisionGroup`

``CreateCollisionGroup(name: `string`)`` → `int`
  [Deprecated]

### `Class.PhysicsService:GetCollisionGroupId`

``GetCollisionGroupId(name: `string`)`` → `int`
  [Deprecated]

### `Class.PhysicsService:GetCollisionGroupName`

``GetCollisionGroupName(name: `int`)`` → `string`
  [Deprecated]

### `Class.PhysicsService:GetCollisionGroups`

``GetCollisionGroups()`` → `Array`
  [Deprecated]

### `Class.PhysicsService:GetMaxCollisionGroups`

``GetMaxCollisionGroups()`` → `int`

### `Class.PhysicsService:GetRegisteredCollisionGroups`

``GetRegisteredCollisionGroups()`` → `Array`

### `Class.PhysicsService:IkSolve`

``IkSolve(part: `Class.BasePart`, target: `Datatype.CFrame`, translateStiffness: `float`, rotateStiffness: `float`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.PhysicsService:IsCollisionGroupRegistered`

``IsCollisionGroupRegistered(name: `string`)`` → `bool`

### `Class.PhysicsService:LocalIkSolve`

``LocalIkSolve(part: `Class.BasePart`, target: `Datatype.CFrame`, translateStiffness: `float`, rotateStiffness: `float`)`` → `null`
   {security: LocalUserSecurity}

### `Class.PhysicsService:RegisterCollisionGroup`

``RegisterCollisionGroup(name: `string`)`` → `null`

### `Class.PhysicsService:RemoveCollisionGroup`

``RemoveCollisionGroup(name: `string`)`` → `null`
  [Deprecated]

### `Class.PhysicsService:RenameCollisionGroup`

``RenameCollisionGroup(from: `string`, to: `string`)`` → `null`

### `Class.PhysicsService:SetPartCollisionGroup`

``SetPartCollisionGroup(part: `Class.BasePart`, name: `string`)`` → `null`
  [Deprecated]

### `Class.PhysicsService:UnregisterCollisionGroup`

``UnregisterCollisionGroup(name: `string`)`` → `null`
