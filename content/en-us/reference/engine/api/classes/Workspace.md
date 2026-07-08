---
title: Workspace
type: class
superclass: WorldRoot
tags: [NotCreatable, Service]
---

# Workspace

`Workspace` houses 3D objects which are rendered to the 3D world. Objects not
descending from it will not be rendered or physically interact with the world.

**Inherits from:** `Class.WorldRoot` > `Class.Model` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

The core job of `Class.Workspace` is to hold objects that exist in the 3D
world, effectively `Class.BasePart|BaseParts` and
`Class.Attachment|Attachments`. While such objects are descendant of
`Class.Workspace`, they will be active. For `Class.BasePart|BaseParts`, this
means they will be rendered, and physically interact with other parts and the
world. For `Class.Attachment|Attachments`, this means that objects adorned to
them, such as `Class.ParticleEmitter|ParticleEmitters`, `Class.Beam|Beams`,
and `Class.BillboardGui|BillboardGuis`, will render.

Understanding this behavior is important, as it means objects can be removed
from `Class.Workspace` when they are not needed. For example, map
`Class.Model|Models` can be removed when a different map is being played on.
Objects that are not immediately needed in the 3D world are generally stored
in `Class.ReplicatedStorage` or `Class.ServerStorage`.

In its role as the holder of active 3D objects, `Class.Workspace` includes a
number of useful functions related to parts, their positions, and joints
between them.

#### Accessing the Workspace

`Class.Workspace` can be accessed several ways, all of which are valid.

- `workspace`
- `game:GetService("Workspace")`
- `game.Workspace`

#### Notes

- Objects that require adornment, such as
  `Class.ParticleEmitter|ParticleEmitters` and
  `Class.BillboardGui|BillboardGuis`, will be at the
  <Typography noWrap>`(0, 0, 0)`</Typography> position when parented to
  `Class.Workspace` without an adornee otherwise being set.
- The `Class.Model:MakeJoints()` and `Class.Model:BreakJoints()` methods
  inherited from the `Class.Model` class are overridden by
  `Class.Workspace:MakeJoints()` and `Class.Workspace:BreakJoints()` which can
  only be used in plugins.
- It is impossible to delete `Class.Workspace`.
- `Class.Workspace` automatically cleans up `Class.BasePart|BaseParts` that
  fall beneath
  `Class.Workspace.FallenPartsDestroyHeight|FallenPartsDestroyHeight`.
- A client's current `Class.Camera` object can be accessed using the
  `Class.Workspace.CurrentCamera` property.
- The `Class.Terrain` object can be accessed using the
  `Class.Workspace.Terrain` property.

## Properties

| Property | Type | Description |
|----------|------|-------------|
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

``ApplyRecommendedStreamingSettings()`` -> `bool`
   {security: PluginSecurity}

### `Class.Workspace:BreakJoints`

``BreakJoints(objects: `Datatype.Instances`)`` -> `null`
  [Deprecated] {security: PluginSecurity}

### `Class.Workspace:CalculateJumpDistance`

``CalculateJumpDistance(gravity: `float`, jumpPower: `float`, walkSpeed: `float`)`` -> `float`
   {security: RobloxScriptSecurity}

### `Class.Workspace:CalculateJumpHeight`

``CalculateJumpHeight(gravity: `float`, jumpPower: `float`)`` -> `float`
   {security: RobloxScriptSecurity}

### `Class.Workspace:CalculateJumpPower`

``CalculateJumpPower(gravity: `float`, jumpHeight: `float`)`` -> `float`
   {security: RobloxScriptSecurity}

### `Class.Workspace:ExperimentalSolverIsEnabled`

``ExperimentalSolverIsEnabled()`` -> `bool`
   {security: LocalUserSecurity}

### `Class.Workspace:GetNumAwakeParts`

``GetNumAwakeParts()`` -> `int`

### `Class.Workspace:GetPhysicsThrottling`

``GetPhysicsThrottling()`` -> `int`

### `Class.Workspace:GetRealPhysicsFPS`

``GetRealPhysicsFPS()`` -> `double`

### `Class.Workspace:GetServerTimeNow`

``GetServerTimeNow()`` -> `double`

### `Class.Workspace:JoinToOutsiders`

``JoinToOutsiders(objects: `Datatype.Instances`, jointType: `Enum.JointCreationMode`)`` -> `null`

### `Class.Workspace:MakeJoints`

``MakeJoints(objects: `Datatype.Instances`)`` -> `null`
  [Deprecated] {security: PluginSecurity}

### `Class.Workspace:PGSIsEnabled`

``PGSIsEnabled()`` -> `bool`

### `Class.Workspace:SetAvatarUnificationMode`

``SetAvatarUnificationMode(value: `Enum.AvatarUnificationMode`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.Workspace:SetMeshPartHeadsAndAccessories`

``SetMeshPartHeadsAndAccessories(value: `Enum.MeshPartHeadsAndAccessories`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.Workspace:SetPhysicsThrottleEnabled`

``SetPhysicsThrottleEnabled(value: `bool`)`` -> `null`
   {security: LocalUserSecurity}

### `Class.Workspace:UnjoinFromOutsiders`

``UnjoinFromOutsiders(objects: `Datatype.Instances`)`` -> `null`

### `Class.Workspace:ZoomToExtents`

``ZoomToExtents()`` -> `null`
   {security: PluginSecurity}

## Events

### `Class.Workspace.PersistentLoaded`

Fires with: (player: `Class.Player`)
