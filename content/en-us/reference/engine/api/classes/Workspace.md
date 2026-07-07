---
title: Workspace
type: class
superclass: WorldRoot
tags: [NotCreatable, Service]
---

# Workspace

**Inherits**: WorldRoot > Model > PVInstance > Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **AirDensity**: `float`
- **AirTurbulenceIntensity**: `float`
- **AllowThirdPartySales**: `bool` [NotReplicated]
- **AuthorityMode**: `AuthorityMode` (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **AvatarUnificationMode**: `AvatarUnificationMode` [NotScriptable]
- **ClientAnimatorThrottling**: `ClientAnimatorThrottlingMode`
- **CurrentCamera**: `Camera` [NotReplicated]
- **DistributedGameTime**: `double` [NotReplicated]
- **EnableSLIMAvatars**: `RolloutState` [NotScriptable]
- **FallHeightEnabled**: `bool` (Security: Read=None, Write=PluginSecurity)
- **FallenPartsDestroyHeight**: `float` (Security: Read=None, Write=PluginSecurity)
- **FilteringEnabled**: `bool` [Hidden] [NotReplicated] [Deprecated] (Security: Read=None, Write=PluginSecurity)
- **FluidForces**: `FluidForces` [NotScriptable]
- **GlobalWind**: `Vector3`
- **Gravity**: `float`
- **IKControlConstraintSupport**: `IKControlConstraintSupport` [NotScriptable]
- **ImprovedAnimationConstraint**: `RolloutState` [NotScriptable]
- **ImprovedPhysicsReplication**: `RolloutState` [NotScriptable]
- **InsertPoint**: `Vector3` [NotReplicated]
- **InterpolationThrottling**: `InterpolationThrottlingMode` [Hidden] [NotReplicated] [Deprecated] (Security: Read=None, Write=PluginSecurity)
- **LayeredClothingCacheOptimizations**: `RolloutState` [NotScriptable]
- **LuauTypeCheckMode**: `LuauTypeCheckMode` (Security: Read=PluginSecurity, Write=PluginSecurity)
- **MeshPartHeadsAndAccessories**: `MeshPartHeadsAndAccessories` [NotScriptable]
- **MeshStreamingAndImprovedLods**: `RolloutState` [NotScriptable]
- **ModelStreamingBehavior**: `ModelStreamingBehavior` [NotScriptable]
- **NextGenerationReplication**: `RolloutState` [NotScriptable]
- **NextGenerationReplicationAlias**: `RolloutState` [NotReplicated] [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **PathfindingUseImprovedSearch**: `PathfindingUseImprovedSearch` [NotScriptable]
- **PhysicsSteppingMethod**: `PhysicsSteppingMethod` [NotScriptable]
- **PlayerCharacterDestroyBehavior**: `PlayerCharacterDestroyBehavior` [NotScriptable]
- **PlayerScriptsUseInputActionSystem**: `RolloutState` [NotScriptable]
- **PlayerScriptsUseInputActionSystemAlias**: `RolloutState` [NotReplicated] [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **PrimalPhysicsSolver**: `PrimalPhysicsSolver` [NotScriptable]
- **RejectCharacterDeletions**: `RejectCharacterDeletions` [NotScriptable]
- **RenderingCacheOptimizations**: `RenderingCacheOptimizationMode` [NotScriptable]
- **ReplicateInstanceDestroySetting**: `ReplicateInstanceDestroySetting` [NotScriptable]
- **Retargeting**: `AnimatorRetargetingMode`
- **SandboxedInstanceMode**: `SandboxedInstanceMode` [NotScriptable]
- **SignalBehavior**: `SignalBehavior` [NotScriptable]
- **SignalBehaviorAlias**: `SignalBehavior` [NotReplicated] [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **StreamOutBehavior**: `StreamOutBehavior` [NotScriptable]
- **StreamingEnabled**: `bool` (Security: Read=None, Write=PluginSecurity)
- **StreamingEnabledAlias**: `bool` [NotReplicated] [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **StreamingIntegrityMode**: `StreamingIntegrityMode` [NotScriptable]
- **StreamingMinRadius**: `int` [NotScriptable]
- **StreamingTargetRadius**: `int` [NotScriptable]
- **Terrain**: `Terrain` [ReadOnly] [NotReplicated]
- **TouchEventsUseCollisionGroups**: `RolloutState` [NotScriptable]
- **TouchesUseCollisionGroups**: `bool` [NotScriptable]
- **UseFixedSimulation**: `RolloutState` [NotScriptable]
- **UseFixedSimulationAlias**: `RolloutState` [NotReplicated] [NotScriptable] (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **UseNewLuauTypeSolver**: `RolloutState` [NotScriptable]
- **ValidateEnabledProximityPrompt**: `RolloutState` [NotScriptable]

## Methods

- **ApplyRecommendedStreamingSettings**() -> `bool`
- **BreakJoints**(`objects: Instances`) -> `null` [Deprecated]
- **CalculateJumpDistance**(`gravity: float`, `jumpPower: float`, `walkSpeed: float`) -> `float`
- **CalculateJumpHeight**(`gravity: float`, `jumpPower: float`) -> `float`
- **CalculateJumpPower**(`gravity: float`, `jumpHeight: float`) -> `float`
- **ExperimentalSolverIsEnabled**() -> `bool`
- **GetNumAwakeParts**() -> `int`
- **GetPhysicsThrottling**() -> `int`
- **GetRealPhysicsFPS**() -> `double`
- **GetServerTimeNow**() -> `double`
- **JoinToOutsiders**(`objects: Instances`, `jointType: JointCreationMode`) -> `null`
- **MakeJoints**(`objects: Instances`) -> `null` [Deprecated]
- **PGSIsEnabled**() -> `bool`
- **SetAvatarUnificationMode**(`value: AvatarUnificationMode`) -> `null`
- **SetMeshPartHeadsAndAccessories**(`value: MeshPartHeadsAndAccessories`) -> `null`
- **SetPhysicsThrottleEnabled**(`value: bool`) -> `null`
- **UnjoinFromOutsiders**(`objects: Instances`) -> `null`
- **ZoomToExtents**() -> `null`

## Events

- **PersistentLoaded**(`player: Player`)
