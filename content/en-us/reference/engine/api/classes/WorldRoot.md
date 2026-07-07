---
title: WorldRoot
type: class
superclass: Model
tags: [NotCreatable]
---

# WorldRoot

**Inherits**: Model > PVInstance > Instance > Object

**Tags**: NotCreatable

## Properties

- **PhysicsStepTime**: `float` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **ArePartsTouchingOthers**(`partList: Instances`, `overlapIgnored: float = 0.000199999995`) -> `bool`
- **Blockcast**(`cframe: CFrame`, `size: Vector3`, `direction: Vector3`, `params: RaycastParams = RaycastParams{IgnoreWater=false, BruteForceAllSlow=false, RespectCanCollide=false, CollisionGroup=Default, FilterDescendantsInstances={}}`) -> `RaycastResult?`
- **BulkMoveTo**(`partList: Instances`, `cframeList: Array`, `eventMode: BulkMoveMode = FireAllEvents`) -> `null`
- **CacheCurrentTerrain**(`id: string`, `center: Vector3`, `radius: float`) -> `string`
- **ClearCachedTerrain**(`id: string`) -> `bool`
- **FindPartOnRay**(`ray: Ray`, `ignoreDescendantsInstance: Instance = nil`, `terrainCellsAreCubes: bool = false`, `ignoreWater: bool = false`) -> `Tuple` [Deprecated]
- **FindPartOnRayWithIgnoreList**(`ray: Ray`, `ignoreDescendantsTable: Instances`, `terrainCellsAreCubes: bool = false`, `ignoreWater: bool = false`) -> `Tuple` [Deprecated]
- **FindPartOnRayWithWhitelist**(`ray: Ray`, `whitelistDescendantsTable: Instances`, `ignoreWater: bool = false`) -> `Tuple` [Deprecated]
- **FindPartsInRegion3**(`region: Region3`, `ignoreDescendantsInstance: Instance = nil`, `maxParts: int = 20`) -> `Instances` [Deprecated]
- **FindPartsInRegion3WithIgnoreList**(`region: Region3`, `ignoreDescendantsTable: Instances`, `maxParts: int = 20`) -> `Instances` [Deprecated]
- **FindPartsInRegion3WithWhiteList**(`region: Region3`, `whitelistDescendantsTable: Instances`, `maxParts: int = 20`) -> `Instances` [Deprecated]
- **GetAwakeContactNormals**() -> `Array` [CustomLuaState]
- **GetAwakeContactParts**() -> `Array` [CustomLuaState]
- **GetAwakeContactPositions**() -> `Array` [CustomLuaState]
- **GetAwakeRootParts**() -> `Instances` [CustomLuaState]
- **GetPartBoundsInBox**(`cframe: CFrame`, `size: Vector3`, `overlapParams: OverlapParams = OverlapParams{MaxParts=0, Tolerance=0, BruteForceAllSlow=false, RespectCanCollide=false, CollisionGroup=Default, FilterDescendantsInstances={}}`) -> `Instances` [CustomLuaState]
- **GetPartBoundsInRadius**(`position: Vector3`, `radius: float`, `overlapParams: OverlapParams = OverlapParams{MaxParts=0, Tolerance=0, BruteForceAllSlow=false, RespectCanCollide=false, CollisionGroup=Default, FilterDescendantsInstances={}}`) -> `Instances` [CustomLuaState]
- **GetPartsInPart**(`part: BasePart`, `overlapParams: OverlapParams = OverlapParams{MaxParts=0, Tolerance=0, BruteForceAllSlow=false, RespectCanCollide=false, CollisionGroup=Default, FilterDescendantsInstances={}}`) -> `Instances` [CustomLuaState]
- **IKMoveTo**(`part: BasePart`, `target: CFrame`, `translateStiffness: float = 0.5`, `rotateStiffness: float = 0.5`, `collisionsMode: IKCollisionsMode = OtherMechanismsAnchored`) -> `null`
- **IsRegion3Empty**(`region: Region3`, `ignoreDescendentsInstance: Instance = nil`) -> `bool` [Deprecated]
- **IsRegion3EmptyWithIgnoreList**(`region: Region3`, `ignoreDescendentsTable: Instances`) -> `bool` [Deprecated]
- **Raycast**(`origin: Vector3`, `direction: Vector3`, `raycastParams: RaycastParams = RaycastParams{IgnoreWater=false, BruteForceAllSlow=false, RespectCanCollide=false, CollisionGroup=Default, FilterDescendantsInstances={}}`) -> `RaycastResult?`
- **RaycastCachedTerrain**(`id: string`, `origin: Vector3`, `direction: Vector3`, `ignoreWater: bool`) -> `RaycastResult?`
- **SetInsertPoint**(`point: Vector3`) -> `null`
- **Shapecast**(`part: BasePart`, `direction: Vector3`, `params: RaycastParams = RaycastParams{IgnoreWater=false, BruteForceAllSlow=false, RespectCanCollide=false, CollisionGroup=Default, FilterDescendantsInstances={}}`) -> `RaycastResult?`
- **Spherecast**(`position: Vector3`, `radius: float`, `direction: Vector3`, `params: RaycastParams = RaycastParams{IgnoreWater=false, BruteForceAllSlow=false, RespectCanCollide=false, CollisionGroup=Default, FilterDescendantsInstances={}}`) -> `RaycastResult?`
- **StepPhysics**(`dt: float`, `parts: Instances = {}`) -> `null`
- **findPartOnRay**(`ray: Ray`, `ignoreDescendantsInstance: Instance = nil`, `terrainCellsAreCubes: bool = false`, `ignoreWater: bool = false`) -> `Tuple` [Deprecated]
- **findPartsInRegion3**(`region: Region3`, `ignoreDescendantsInstance: Instance = nil`, `maxParts: int = 20`) -> `Instances` [Deprecated]
