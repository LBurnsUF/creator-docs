---
title: WorldRoot
type: class
superclass: Model
tags: [NotCreatable]
---

# WorldRoot

**Inherits from:** `Class.Model` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.WorldRoot.PhysicsStepTime` | `float` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |

## Methods

### `Class.WorldRoot:ArePartsTouchingOthers`

``ArePartsTouchingOthers(partList: `Datatype.Instances`, overlapIgnored: `float`)`` → `bool`

### `Class.WorldRoot:Blockcast`

``Blockcast(cframe: `Datatype.CFrame`, size: `Datatype.Vector3`, direction: `Datatype.Vector3`, params: `Datatype.RaycastParams`)`` → `Datatype.RaycastResult`?

### `Class.WorldRoot:BulkMoveTo`

``BulkMoveTo(partList: `Datatype.Instances`, cframeList: `Array`, eventMode: `Enum.BulkMoveMode`)`` → `null`

### `Class.WorldRoot:CacheCurrentTerrain`

``CacheCurrentTerrain(id: `string`, center: `Datatype.Vector3`, radius: `float`)`` → `string`
   {security: RobloxScriptSecurity}

### `Class.WorldRoot:ClearCachedTerrain`

``ClearCachedTerrain(id: `string`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.WorldRoot:FindPartOnRay`

``FindPartOnRay(ray: `Datatype.Ray`, ignoreDescendantsInstance: `Class.Instance`, terrainCellsAreCubes: `bool`, ignoreWater: `bool`)`` → `Tuple`
  [Deprecated]

### `Class.WorldRoot:FindPartOnRayWithIgnoreList`

``FindPartOnRayWithIgnoreList(ray: `Datatype.Ray`, ignoreDescendantsTable: `Datatype.Instances`, terrainCellsAreCubes: `bool`, ignoreWater: `bool`)`` → `Tuple`
  [Deprecated]

### `Class.WorldRoot:FindPartOnRayWithWhitelist`

``FindPartOnRayWithWhitelist(ray: `Datatype.Ray`, whitelistDescendantsTable: `Datatype.Instances`, ignoreWater: `bool`)`` → `Tuple`
  [Deprecated]

### `Class.WorldRoot:FindPartsInRegion3`

``FindPartsInRegion3(region: `Datatype.Region3`, ignoreDescendantsInstance: `Class.Instance`, maxParts: `int`)`` → `Datatype.Instances`
  [Deprecated]

### `Class.WorldRoot:FindPartsInRegion3WithIgnoreList`

``FindPartsInRegion3WithIgnoreList(region: `Datatype.Region3`, ignoreDescendantsTable: `Datatype.Instances`, maxParts: `int`)`` → `Datatype.Instances`
  [Deprecated]

### `Class.WorldRoot:FindPartsInRegion3WithWhiteList`

``FindPartsInRegion3WithWhiteList(region: `Datatype.Region3`, whitelistDescendantsTable: `Datatype.Instances`, maxParts: `int`)`` → `Datatype.Instances`
  [Deprecated]

### `Class.WorldRoot:GetAwakeContactNormals`

``GetAwakeContactNormals()`` → `Array`
  [CustomLuaState] {security: RobloxScriptSecurity}

### `Class.WorldRoot:GetAwakeContactParts`

``GetAwakeContactParts()`` → `Array`
  [CustomLuaState] {security: RobloxScriptSecurity}

### `Class.WorldRoot:GetAwakeContactPositions`

``GetAwakeContactPositions()`` → `Array`
  [CustomLuaState] {security: RobloxScriptSecurity}

### `Class.WorldRoot:GetAwakeRootParts`

``GetAwakeRootParts()`` → `Datatype.Instances`
  [CustomLuaState] {security: RobloxScriptSecurity}

### `Class.WorldRoot:GetPartBoundsInBox`

``GetPartBoundsInBox(cframe: `Datatype.CFrame`, size: `Datatype.Vector3`, overlapParams: `Datatype.OverlapParams`)`` → `Datatype.Instances`
  [CustomLuaState]

### `Class.WorldRoot:GetPartBoundsInRadius`

``GetPartBoundsInRadius(position: `Datatype.Vector3`, radius: `float`, overlapParams: `Datatype.OverlapParams`)`` → `Datatype.Instances`
  [CustomLuaState]

### `Class.WorldRoot:GetPartsInPart`

``GetPartsInPart(part: `Class.BasePart`, overlapParams: `Datatype.OverlapParams`)`` → `Datatype.Instances`
  [CustomLuaState]

### `Class.WorldRoot:IKMoveTo`

``IKMoveTo(part: `Class.BasePart`, target: `Datatype.CFrame`, translateStiffness: `float`, rotateStiffness: `float`, collisionsMode: `Enum.IKCollisionsMode`)`` → `null`
   {security: PluginSecurity}

### `Class.WorldRoot:IsRegion3Empty`

``IsRegion3Empty(region: `Datatype.Region3`, ignoreDescendentsInstance: `Class.Instance`)`` → `bool`
  [Deprecated]

### `Class.WorldRoot:IsRegion3EmptyWithIgnoreList`

``IsRegion3EmptyWithIgnoreList(region: `Datatype.Region3`, ignoreDescendentsTable: `Datatype.Instances`)`` → `bool`
  [Deprecated]

### `Class.WorldRoot:Raycast`

``Raycast(origin: `Datatype.Vector3`, direction: `Datatype.Vector3`, raycastParams: `Datatype.RaycastParams`)`` → `Datatype.RaycastResult`?

### `Class.WorldRoot:RaycastCachedTerrain`

``RaycastCachedTerrain(id: `string`, origin: `Datatype.Vector3`, direction: `Datatype.Vector3`, ignoreWater: `bool`)`` → `Datatype.RaycastResult`?
   {security: RobloxScriptSecurity}

### `Class.WorldRoot:SetInsertPoint`

``SetInsertPoint(point: `Datatype.Vector3`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.WorldRoot:Shapecast`

``Shapecast(part: `Class.BasePart`, direction: `Datatype.Vector3`, params: `Datatype.RaycastParams`)`` → `Datatype.RaycastResult`?

### `Class.WorldRoot:Spherecast`

``Spherecast(position: `Datatype.Vector3`, radius: `float`, direction: `Datatype.Vector3`, params: `Datatype.RaycastParams`)`` → `Datatype.RaycastResult`?

### `Class.WorldRoot:StepPhysics`

``StepPhysics(dt: `float`, parts: `Datatype.Instances`)`` → `null`
   {security: PluginSecurity}

### `Class.WorldRoot:findPartOnRay`

``findPartOnRay(ray: `Datatype.Ray`, ignoreDescendantsInstance: `Class.Instance`, terrainCellsAreCubes: `bool`, ignoreWater: `bool`)`` → `Tuple`
  [Deprecated]

### `Class.WorldRoot:findPartsInRegion3`

``findPartsInRegion3(region: `Datatype.Region3`, ignoreDescendantsInstance: `Class.Instance`, maxParts: `int`)`` → `Datatype.Instances`
  [Deprecated]
