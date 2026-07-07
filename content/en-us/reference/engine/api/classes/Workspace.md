---
title: Workspace
type: class
superclass: WorldRoot
tags: [NotCreatable, Service]
---

# Workspace

**Inherits from:** `Class.WorldRoot` > `Class.Model` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.Workspace.AirDensity` | `float` |  |
| `Class.Workspace.AirTurbulenceIntensity` | `float` |  |
| `Class.Workspace.AllowThirdPartySales` | `bool` | [NotReplicated] |
| `Class.Workspace.AuthorityMode` | `Enum.AuthorityMode` |  {security: RobloxScriptSecurity} |
| `Class.Workspace.AvatarUnificationMode` | `Enum.AvatarUnificationMode` | [NotScriptable] |
| `Class.Workspace.ClientAnimatorThrottling` | `Enum.ClientAnimatorThrottlingMode` |  |
| `Class.Workspace.CurrentCamera` | `Class.Camera` | [NotReplicated] |
| `Class.Workspace.DistributedGameTime` | `double` | [NotReplicated] |
| `Class.Workspace.EnableSLIMAvatars` | `Enum.RolloutState` | [NotScriptable] |
| `Class.Workspace.FallHeightEnabled` | `bool` |  {write: PluginSecurity} |
| `Class.Workspace.FallenPartsDestroyHeight` | `float` |  {write: PluginSecurity} |
| `Class.Workspace.FilteringEnabled` | `bool` | [Hidden] [NotReplicated] [Deprecated] {write: PluginSecurity} |
| `Class.Workspace.FluidForces` | `Enum.FluidForces` | [NotScriptable] |
| `Class.Workspace.GlobalWind` | `Datatype.Vector3` |  |
| `Class.Workspace.Gravity` | `float` |  |
| `Class.Workspace.IKControlConstraintSupport` | `Enum.IKControlConstraintSupport` | [NotScriptable] |
| `Class.Workspace.ImprovedAnimationConstraint` | `Enum.RolloutState` | [NotScriptable] |
| `Class.Workspace.ImprovedPhysicsReplication` | `Enum.RolloutState` | [NotScriptable] |
| `Class.Workspace.InsertPoint` | `Datatype.Vector3` | [NotReplicated] |
| `Class.Workspace.InterpolationThrottling` | `Enum.InterpolationThrottlingMode` | [Hidden] [NotReplicated] [Deprecated] {write: PluginSecurity} |
| `Class.Workspace.LayeredClothingCacheOptimizations` | `Enum.RolloutState` | [NotScriptable] |
| `Class.Workspace.LuauTypeCheckMode` | `Enum.LuauTypeCheckMode` |  {security: PluginSecurity} |
| `Class.Workspace.MeshPartHeadsAndAccessories` | `Enum.MeshPartHeadsAndAccessories` | [NotScriptable] |
| `Class.Workspace.MeshStreamingAndImprovedLods` | `Enum.RolloutState` | [NotScriptable] |
| `Class.Workspace.ModelStreamingBehavior` | `Enum.ModelStreamingBehavior` | [NotScriptable] |
| `Class.Workspace.NextGenerationReplication` | `Enum.RolloutState` | [NotScriptable] |
| `Class.Workspace.NextGenerationReplicationAlias` | `Enum.RolloutState` | [NotReplicated] [NotScriptable] {security: RobloxSecurity} |
| `Class.Workspace.PathfindingUseImprovedSearch` | `Enum.PathfindingUseImprovedSearch` | [NotScriptable] |
| `Class.Workspace.PhysicsSteppingMethod` | `Enum.PhysicsSteppingMethod` | [NotScriptable] |
| `Class.Workspace.PlayerCharacterDestroyBehavior` | `Enum.PlayerCharacterDestroyBehavior` | [NotScriptable] |
| `Class.Workspace.PlayerScriptsUseInputActionSystem` | `Enum.RolloutState` | [NotScriptable] |
| `Class.Workspace.PlayerScriptsUseInputActionSystemAlias` | `Enum.RolloutState` | [NotReplicated] [NotScriptable] {security: RobloxSecurity} |
| `Class.Workspace.PrimalPhysicsSolver` | `Enum.PrimalPhysicsSolver` | [NotScriptable] |
| `Class.Workspace.RejectCharacterDeletions` | `Enum.RejectCharacterDeletions` | [NotScriptable] |
| `Class.Workspace.RenderingCacheOptimizations` | `Enum.RenderingCacheOptimizationMode` | [NotScriptable] |
| `Class.Workspace.ReplicateInstanceDestroySetting` | `Enum.ReplicateInstanceDestroySetting` | [NotScriptable] |
| `Class.Workspace.Retargeting` | `Enum.AnimatorRetargetingMode` |  |
| `Class.Workspace.SandboxedInstanceMode` | `Enum.SandboxedInstanceMode` | [NotScriptable] |
| `Class.Workspace.SignalBehavior` | `Enum.SignalBehavior` | [NotScriptable] |
| `Class.Workspace.SignalBehaviorAlias` | `Enum.SignalBehavior` | [NotReplicated] [NotScriptable] {security: RobloxSecurity} |
| `Class.Workspace.StreamOutBehavior` | `Enum.StreamOutBehavior` | [NotScriptable] |
| `Class.Workspace.StreamingEnabled` | `bool` |  {write: PluginSecurity} |
| `Class.Workspace.StreamingEnabledAlias` | `bool` | [NotReplicated] [NotScriptable] {security: RobloxSecurity} |
| `Class.Workspace.StreamingIntegrityMode` | `Enum.StreamingIntegrityMode` | [NotScriptable] |
| `Class.Workspace.StreamingMinRadius` | `int` | [NotScriptable] |
| `Class.Workspace.StreamingTargetRadius` | `int` | [NotScriptable] |
| `Class.Workspace.Terrain` | `Class.Terrain` | [ReadOnly] [NotReplicated] |
| `Class.Workspace.TouchEventsUseCollisionGroups` | `Enum.RolloutState` | [NotScriptable] |
| `Class.Workspace.TouchesUseCollisionGroups` | `bool` | [NotScriptable] |
| `Class.Workspace.UseFixedSimulation` | `Enum.RolloutState` | [NotScriptable] |
| `Class.Workspace.UseFixedSimulationAlias` | `Enum.RolloutState` | [NotReplicated] [NotScriptable] {security: RobloxSecurity} |
| `Class.Workspace.UseNewLuauTypeSolver` | `Enum.RolloutState` | [NotScriptable] |
| `Class.Workspace.ValidateEnabledProximityPrompt` | `Enum.RolloutState` | [NotScriptable] |

## Methods

### `Class.Workspace:ApplyRecommendedStreamingSettings`

``ApplyRecommendedStreamingSettings()`` → `bool`
   {security: PluginSecurity}

### `Class.Workspace:BreakJoints`

``BreakJoints(objects: `Datatype.Instances`)`` → `null`
  [Deprecated] {security: PluginSecurity}

### `Class.Workspace:CalculateJumpDistance`

``CalculateJumpDistance(gravity: `float`, jumpPower: `float`, walkSpeed: `float`)`` → `float`
   {security: RobloxScriptSecurity}

### `Class.Workspace:CalculateJumpHeight`

``CalculateJumpHeight(gravity: `float`, jumpPower: `float`)`` → `float`
   {security: RobloxScriptSecurity}

### `Class.Workspace:CalculateJumpPower`

``CalculateJumpPower(gravity: `float`, jumpHeight: `float`)`` → `float`
   {security: RobloxScriptSecurity}

### `Class.Workspace:ExperimentalSolverIsEnabled`

``ExperimentalSolverIsEnabled()`` → `bool`
   {security: LocalUserSecurity}

### `Class.Workspace:GetNumAwakeParts`

``GetNumAwakeParts()`` → `int`

### `Class.Workspace:GetPhysicsThrottling`

``GetPhysicsThrottling()`` → `int`

### `Class.Workspace:GetRealPhysicsFPS`

``GetRealPhysicsFPS()`` → `double`

### `Class.Workspace:GetServerTimeNow`

``GetServerTimeNow()`` → `double`

### `Class.Workspace:JoinToOutsiders`

``JoinToOutsiders(objects: `Datatype.Instances`, jointType: `Enum.JointCreationMode`)`` → `null`

### `Class.Workspace:MakeJoints`

``MakeJoints(objects: `Datatype.Instances`)`` → `null`
  [Deprecated] {security: PluginSecurity}

### `Class.Workspace:PGSIsEnabled`

``PGSIsEnabled()`` → `bool`

### `Class.Workspace:SetAvatarUnificationMode`

``SetAvatarUnificationMode(value: `Enum.AvatarUnificationMode`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Workspace:SetMeshPartHeadsAndAccessories`

``SetMeshPartHeadsAndAccessories(value: `Enum.MeshPartHeadsAndAccessories`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Workspace:SetPhysicsThrottleEnabled`

``SetPhysicsThrottleEnabled(value: `bool`)`` → `null`
   {security: LocalUserSecurity}

### `Class.Workspace:UnjoinFromOutsiders`

``UnjoinFromOutsiders(objects: `Datatype.Instances`)`` → `null`

### `Class.Workspace:ZoomToExtents`

``ZoomToExtents()`` → `null`
   {security: PluginSecurity}

## Events

### `Class.Workspace.PersistentLoaded`

Fires with: (player: `Class.Player`)
