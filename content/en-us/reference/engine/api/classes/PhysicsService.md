---
title: PhysicsService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# PhysicsService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **CollisionGroupContainsPart**(`name: string`, `part: BasePart`) -> `bool` [Deprecated]
- **CollisionGroupSetCollidable**(`name1: string`, `name2: string`, `collidable: bool`) -> `null`
- **CollisionGroupsAreCollidable**(`name1: string`, `name2: string`) -> `bool`
- **CreateCollisionGroup**(`name: string`) -> `int` [Deprecated]
- **GetCollisionGroupId**(`name: string`) -> `int` [Deprecated]
- **GetCollisionGroupName**(`name: int`) -> `string` [Deprecated]
- **GetCollisionGroups**() -> `Array` [Deprecated]
- **GetMaxCollisionGroups**() -> `int`
- **GetRegisteredCollisionGroups**() -> `Array`
- **IkSolve**(`part: BasePart`, `target: CFrame`, `translateStiffness: float`, `rotateStiffness: float`) -> `null`
- **IsCollisionGroupRegistered**(`name: string`) -> `bool`
- **LocalIkSolve**(`part: BasePart`, `target: CFrame`, `translateStiffness: float`, `rotateStiffness: float`) -> `null`
- **RegisterCollisionGroup**(`name: string`) -> `null`
- **RemoveCollisionGroup**(`name: string`) -> `null` [Deprecated]
- **RenameCollisionGroup**(`from: string`, `to: string`) -> `null`
- **SetPartCollisionGroup**(`part: BasePart`, `name: string`) -> `null` [Deprecated]
- **UnregisterCollisionGroup**(`name: string`) -> `null`
