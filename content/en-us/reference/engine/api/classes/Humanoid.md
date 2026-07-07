---
title: Humanoid
type: class
superclass: Instance
---

# Humanoid

**Inherits**: Instance > Object

## Properties

- **AutoJumpEnabled**: `bool`
- **AutoRotate**: `bool`
- **AutomaticScalingEnabled**: `bool`
- **BreakJointsOnDeath**: `bool`
- **CameraOffset**: `Vector3`
- **CollisionType**: `HumanoidCollisionType` [Deprecated] (Security: Read=None, Write=PluginSecurity)
- **DisplayDistanceType**: `HumanoidDisplayDistanceType`
- **DisplayName**: `string`
- **EvaluateStateMachine**: `bool`
- **FloorMaterial**: `Material` [ReadOnly] [NotReplicated]
- **Health**: `float` [NotReplicated]
- **HealthDisplayDistance**: `float`
- **HealthDisplayType**: `HumanoidHealthDisplayType`
- **HipHeight**: `float`
- **InternalDisplayName**: `string` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Jump**: `bool` [NotReplicated]
- **JumpHeight**: `float`
- **JumpPower**: `float`
- **LeftLeg**: `BasePart` [Hidden] [NotReplicated] [Deprecated]
- **MaxHealth**: `float`
- **MaxSlopeAngle**: `float`
- **MoveDirection**: `Vector3` [ReadOnly] [NotReplicated]
- **NameDisplayDistance**: `float`
- **NameOcclusion**: `NameOcclusion`
- **PlatformStand**: `bool`
- **RequiresNeck**: `bool`
- **RigType**: `HumanoidRigType`
- **RightLeg**: `BasePart` [Hidden] [NotReplicated] [Deprecated]
- **RootPart**: `BasePart` [ReadOnly] [NotReplicated]
- **SeatPart**: `BasePart` [ReadOnly] [NotReplicated]
- **Sit**: `bool`
- **TargetPoint**: `Vector3`
- **Torso**: `BasePart` [Hidden] [NotReplicated] [Deprecated]
- **UseJumpPower**: `bool`
- **WalkSpeed**: `float`
- **WalkToPart**: `BasePart`
- **WalkToPoint**: `Vector3`
- **maxHealth**: `float` [NotReplicated] [Deprecated]

## Methods

- **AddAccessory**(`accessory: Instance`) -> `null`
- **AddCustomStatus**(`status: string`) -> `bool` [Deprecated]
- **AddStatus**(`status: Status = Poison`) -> `bool` [Deprecated]
- **ApplyAvatarRules**(`avatarRules: AvatarRules`) -> `null` [Yields]
- **ApplyDescription**(`humanoidDescription: HumanoidDescription`, `assetTypeVerification: AssetTypeVerification = Default`) -> `null` [Yields] [Deprecated]
- **ApplyDescriptionAsync**(`humanoidDescription: HumanoidDescription`, `assetTypeVerification: AssetTypeVerification = Default`) -> `null` [Yields]
- **ApplyDescriptionReset**(`humanoidDescription: HumanoidDescription`, `assetTypeVerification: AssetTypeVerification = Default`) -> `null` [Yields] [Deprecated]
- **ApplyDescriptionResetAsync**(`humanoidDescription: HumanoidDescription`, `assetTypeVerification: AssetTypeVerification = Default`) -> `null` [Yields]
- **BuildRigFromAttachments**() -> `null`
- **CacheDefaults**() -> `null`
- **ChangeState**(`state: HumanoidStateType = None`) -> `null`
- **ComputeOriginalSizeForPart**(`part: Instance`) -> `Vector3?`
- **ComputeR15BodyBoundingBox**() -> `[{'Category': 'DataType', 'Name': 'CFrame'}, {'Category': 'DataType', 'Name': 'Vector3'}]`
- **EquipTool**(`tool: Instance`) -> `null`
- **GetAccessories**() -> `Array`
- **GetAccessoryHandleScale**(`instance: Instance`, `partType: BodyPartR15`) -> `Vector3`
- **GetAppliedDescription**() -> `HumanoidDescription`
- **GetBodyPartR15**(`part: Instance`) -> `BodyPartR15`
- **GetLimb**(`part: Instance`) -> `Limb`
- **GetMoveVelocity**() -> `Vector3`
- **GetPlayingAnimationTracks**() -> `Array` [Deprecated]
- **GetRelativeVelocityAtFloor**() -> `Vector3`
- **GetState**() -> `HumanoidStateType`
- **GetStateEnabled**(`state: HumanoidStateType`) -> `bool`
- **GetStatuses**() -> `Array` [Deprecated]
- **HasCustomStatus**(`status: string`) -> `bool` [Deprecated]
- **HasStatus**(`status: Status = Poison`) -> `bool` [Deprecated]
- **LoadAnimation**(`animation: Animation`) -> `AnimationTrack` [Deprecated]
- **Move**(`moveDirection: Vector3`, `relativeToCamera: bool = false`) -> `null`
- **MoveTo**(`location: Vector3`, `part: Instance = nil`) -> `null`
- **PlayEmote**(`emoteName: string`) -> `bool` [Yields] [Deprecated]
- **PlayEmoteAndGetAnimTrackById**(`emoteId: int64`) -> `Tuple` [Yields]
- **PlayEmoteAsync**(`emoteName: string`) -> `bool` [Yields]
- **RemoveAccessories**() -> `null`
- **RemoveCustomStatus**(`status: string`) -> `bool` [Deprecated]
- **RemoveStatus**(`status: Status = Poison`) -> `bool` [Deprecated]
- **ReplaceBodyPartR15**(`bodyPart: BodyPartR15`, `part: BasePart`) -> `bool`
- **SetClickToWalkEnabled**(`enabled: bool`) -> `null`
- **SetStateEnabled**(`state: HumanoidStateType`, `enabled: bool`) -> `null`
- **TakeDamage**(`amount: float`) -> `null`
- **UnequipTools**() -> `null`
- **loadAnimation**(`animation: Animation`) -> `AnimationTrack` [Deprecated]
- **takeDamage**(`amount: float`) -> `null` [Deprecated]

## Events

- **AnimationPlayed**(`animationTrack: AnimationTrack`) [Deprecated]
- **ApplyDescriptionFinished**(`description: HumanoidDescription`)
- **Climbing**(`speed: float`)
- **ClusterCompositionFinished**()
- **CustomStatusAdded**(`status: string`) [Deprecated]
- **CustomStatusRemoved**(`status: string`) [Deprecated]
- **Died**()
- **EmoteTriggered**(`success: bool`, `animationTrack: AnimationTrack`)
- **FallingDown**(`active: bool`)
- **FreeFalling**(`active: bool`)
- **GettingUp**(`active: bool`)
- **HealthChanged**(`health: float`)
- **Jumping**(`active: bool`)
- **MoveToFinished**(`reached: bool`)
- **PlatformStanding**(`active: bool`)
- **Ragdoll**(`active: bool`)
- **Running**(`speed: float`)
- **Seated**(`active: bool`, `currentSeatPart: BasePart`)
- **StateChanged**(`old: HumanoidStateType`, `new: HumanoidStateType`)
- **StateEnabledChanged**(`state: HumanoidStateType`, `isEnabled: bool`)
- **StatusAdded**(`status: Status`) [Deprecated]
- **StatusRemoved**(`status: Status`) [Deprecated]
- **Strafing**(`active: bool`)
- **Swimming**(`speed: float`)
- **Touched**(`touchingPart: BasePart`, `humanoidPart: BasePart`)
