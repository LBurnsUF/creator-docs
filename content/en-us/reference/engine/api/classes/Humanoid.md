---
title: Humanoid
type: class
superclass: Instance
---

# Humanoid

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.Humanoid.AutoJumpEnabled` | `bool` |  |
| `Class.Humanoid.AutoRotate` | `bool` |  |
| `Class.Humanoid.AutomaticScalingEnabled` | `bool` |  |
| `Class.Humanoid.BreakJointsOnDeath` | `bool` |  |
| `Class.Humanoid.CameraOffset` | `Datatype.Vector3` |  |
| `Class.Humanoid.CollisionType` | `Enum.HumanoidCollisionType` | [Deprecated] {write: PluginSecurity} |
| `Class.Humanoid.DisplayDistanceType` | `Enum.HumanoidDisplayDistanceType` |  |
| `Class.Humanoid.DisplayName` | `string` |  |
| `Class.Humanoid.EvaluateStateMachine` | `bool` |  |
| `Class.Humanoid.FloorMaterial` | `Enum.Material` | [ReadOnly] [NotReplicated] |
| `Class.Humanoid.Health` | `float` | [NotReplicated] |
| `Class.Humanoid.HealthDisplayDistance` | `float` |  |
| `Class.Humanoid.HealthDisplayType` | `Enum.HumanoidHealthDisplayType` |  |
| `Class.Humanoid.HipHeight` | `float` |  |
| `Class.Humanoid.InternalDisplayName` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Humanoid.Jump` | `bool` | [NotReplicated] |
| `Class.Humanoid.JumpHeight` | `float` |  |
| `Class.Humanoid.JumpPower` | `float` |  |
| `Class.Humanoid.LeftLeg` | `Class.BasePart` | [Hidden] [NotReplicated] [Deprecated] |
| `Class.Humanoid.MaxHealth` | `float` |  |
| `Class.Humanoid.MaxSlopeAngle` | `float` |  |
| `Class.Humanoid.MoveDirection` | `Datatype.Vector3` | [ReadOnly] [NotReplicated] |
| `Class.Humanoid.NameDisplayDistance` | `float` |  |
| `Class.Humanoid.NameOcclusion` | `Enum.NameOcclusion` |  |
| `Class.Humanoid.PlatformStand` | `bool` |  |
| `Class.Humanoid.RequiresNeck` | `bool` |  |
| `Class.Humanoid.RigType` | `Enum.HumanoidRigType` |  |
| `Class.Humanoid.RightLeg` | `Class.BasePart` | [Hidden] [NotReplicated] [Deprecated] |
| `Class.Humanoid.RootPart` | `Class.BasePart` | [ReadOnly] [NotReplicated] |
| `Class.Humanoid.SeatPart` | `Class.BasePart` | [ReadOnly] [NotReplicated] |
| `Class.Humanoid.Sit` | `bool` |  |
| `Class.Humanoid.TargetPoint` | `Datatype.Vector3` |  |
| `Class.Humanoid.Torso` | `Class.BasePart` | [Hidden] [NotReplicated] [Deprecated] |
| `Class.Humanoid.UseJumpPower` | `bool` |  |
| `Class.Humanoid.WalkSpeed` | `float` |  |
| `Class.Humanoid.WalkToPart` | `Class.BasePart` |  |
| `Class.Humanoid.WalkToPoint` | `Datatype.Vector3` |  |
| `Class.Humanoid.maxHealth` | `float` | [NotReplicated] [Deprecated] |

## Methods

### `Class.Humanoid:AddAccessory`

``AddAccessory(accessory: `Class.Instance`)`` → `null`

### `Class.Humanoid:AddCustomStatus`

``AddCustomStatus(status: `string`)`` → `bool`
  [Deprecated]

### `Class.Humanoid:AddStatus`

``AddStatus(status: `Enum.Status`)`` → `bool`
  [Deprecated]

### `Class.Humanoid:ApplyAvatarRules`

``ApplyAvatarRules(avatarRules: `Class.AvatarRules`)`` → `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.Humanoid:ApplyDescription`

``ApplyDescription(humanoidDescription: `Class.HumanoidDescription`, assetTypeVerification: `Enum.AssetTypeVerification`)`` → `null`
  [Yields] [Deprecated]

### `Class.Humanoid:ApplyDescriptionAsync`

``ApplyDescriptionAsync(humanoidDescription: `Class.HumanoidDescription`, assetTypeVerification: `Enum.AssetTypeVerification`)`` → `null`
  [Yields]

### `Class.Humanoid:ApplyDescriptionReset`

``ApplyDescriptionReset(humanoidDescription: `Class.HumanoidDescription`, assetTypeVerification: `Enum.AssetTypeVerification`)`` → `null`
  [Yields] [Deprecated]

### `Class.Humanoid:ApplyDescriptionResetAsync`

``ApplyDescriptionResetAsync(humanoidDescription: `Class.HumanoidDescription`, assetTypeVerification: `Enum.AssetTypeVerification`)`` → `null`
  [Yields]

### `Class.Humanoid:BuildRigFromAttachments`

``BuildRigFromAttachments()`` → `null`

### `Class.Humanoid:CacheDefaults`

``CacheDefaults()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Humanoid:ChangeState`

``ChangeState(state: `Enum.HumanoidStateType`)`` → `null`

### `Class.Humanoid:ComputeOriginalSizeForPart`

``ComputeOriginalSizeForPart(part: `Class.Instance`)`` → `Datatype.Vector3`?
   {security: RobloxScriptSecurity}

### `Class.Humanoid:ComputeR15BodyBoundingBox`

``ComputeR15BodyBoundingBox()`` → `[{'Category': 'DataType', 'Name': 'CFrame'}, {'Category': 'DataType', 'Name': 'Vector3'}]`
   {security: RobloxScriptSecurity}

### `Class.Humanoid:EquipTool`

``EquipTool(tool: `Class.Instance`)`` → `null`

### `Class.Humanoid:GetAccessories`

``GetAccessories()`` → `Array`

### `Class.Humanoid:GetAccessoryHandleScale`

``GetAccessoryHandleScale(instance: `Class.Instance`, partType: `Enum.BodyPartR15`)`` → `Datatype.Vector3`
   {security: RobloxScriptSecurity}

### `Class.Humanoid:GetAppliedDescription`

``GetAppliedDescription()`` → `Class.HumanoidDescription`

### `Class.Humanoid:GetBodyPartR15`

``GetBodyPartR15(part: `Class.Instance`)`` → `Enum.BodyPartR15`

### `Class.Humanoid:GetLimb`

``GetLimb(part: `Class.Instance`)`` → `Enum.Limb`

### `Class.Humanoid:GetMoveVelocity`

``GetMoveVelocity()`` → `Datatype.Vector3`

### `Class.Humanoid:GetPlayingAnimationTracks`

``GetPlayingAnimationTracks()`` → `Array`
  [Deprecated]

### `Class.Humanoid:GetRelativeVelocityAtFloor`

``GetRelativeVelocityAtFloor()`` → `Datatype.Vector3`

### `Class.Humanoid:GetState`

``GetState()`` → `Enum.HumanoidStateType`

### `Class.Humanoid:GetStateEnabled`

``GetStateEnabled(state: `Enum.HumanoidStateType`)`` → `bool`

### `Class.Humanoid:GetStatuses`

``GetStatuses()`` → `Array`
  [Deprecated]

### `Class.Humanoid:HasCustomStatus`

``HasCustomStatus(status: `string`)`` → `bool`
  [Deprecated]

### `Class.Humanoid:HasStatus`

``HasStatus(status: `Enum.Status`)`` → `bool`
  [Deprecated]

### `Class.Humanoid:LoadAnimation`

``LoadAnimation(animation: `Class.Animation`)`` → `Class.AnimationTrack`
  [Deprecated]

### `Class.Humanoid:Move`

``Move(moveDirection: `Datatype.Vector3`, relativeToCamera: `bool`)`` → `null`

### `Class.Humanoid:MoveTo`

``MoveTo(location: `Datatype.Vector3`, part: `Class.Instance`)`` → `null`

### `Class.Humanoid:PlayEmote`

``PlayEmote(emoteName: `string`)`` → `bool`
  [Yields] [Deprecated]

### `Class.Humanoid:PlayEmoteAndGetAnimTrackById`

``PlayEmoteAndGetAnimTrackById(emoteId: `int64`)`` → `Tuple`
  [Yields] {security: RobloxScriptSecurity}

### `Class.Humanoid:PlayEmoteAsync`

``PlayEmoteAsync(emoteName: `string`)`` → `bool`
  [Yields]

### `Class.Humanoid:RemoveAccessories`

``RemoveAccessories()`` → `null`

### `Class.Humanoid:RemoveCustomStatus`

``RemoveCustomStatus(status: `string`)`` → `bool`
  [Deprecated]

### `Class.Humanoid:RemoveStatus`

``RemoveStatus(status: `Enum.Status`)`` → `bool`
  [Deprecated]

### `Class.Humanoid:ReplaceBodyPartR15`

``ReplaceBodyPartR15(bodyPart: `Enum.BodyPartR15`, part: `Class.BasePart`)`` → `bool`

### `Class.Humanoid:SetClickToWalkEnabled`

``SetClickToWalkEnabled(enabled: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Humanoid:SetStateEnabled`

``SetStateEnabled(state: `Enum.HumanoidStateType`, enabled: `bool`)`` → `null`

### `Class.Humanoid:TakeDamage`

``TakeDamage(amount: `float`)`` → `null`

### `Class.Humanoid:UnequipTools`

``UnequipTools()`` → `null`

### `Class.Humanoid:loadAnimation`

``loadAnimation(animation: `Class.Animation`)`` → `Class.AnimationTrack`
  [Deprecated]

### `Class.Humanoid:takeDamage`

``takeDamage(amount: `float`)`` → `null`
  [Deprecated]

## Events

### `Class.Humanoid.AnimationPlayed`

Fires with: (animationTrack: `Class.AnimationTrack`)
  [Deprecated]

### `Class.Humanoid.ApplyDescriptionFinished`

Fires with: (description: `Class.HumanoidDescription`)

### `Class.Humanoid.Climbing`

Fires with: (speed: `float`)

### `Class.Humanoid.ClusterCompositionFinished`

Fires with: ()

### `Class.Humanoid.CustomStatusAdded`

Fires with: (status: `string`)
  [Deprecated]

### `Class.Humanoid.CustomStatusRemoved`

Fires with: (status: `string`)
  [Deprecated]

### `Class.Humanoid.Died`

Fires with: ()

### `Class.Humanoid.EmoteTriggered`

Fires with: (success: `bool`, animationTrack: `Class.AnimationTrack`)

### `Class.Humanoid.FallingDown`

Fires with: (active: `bool`)

### `Class.Humanoid.FreeFalling`

Fires with: (active: `bool`)

### `Class.Humanoid.GettingUp`

Fires with: (active: `bool`)

### `Class.Humanoid.HealthChanged`

Fires with: (health: `float`)

### `Class.Humanoid.Jumping`

Fires with: (active: `bool`)

### `Class.Humanoid.MoveToFinished`

Fires with: (reached: `bool`)

### `Class.Humanoid.PlatformStanding`

Fires with: (active: `bool`)

### `Class.Humanoid.Ragdoll`

Fires with: (active: `bool`)

### `Class.Humanoid.Running`

Fires with: (speed: `float`)

### `Class.Humanoid.Seated`

Fires with: (active: `bool`, currentSeatPart: `Class.BasePart`)

### `Class.Humanoid.StateChanged`

Fires with: (old: `Enum.HumanoidStateType`, new: `Enum.HumanoidStateType`)

### `Class.Humanoid.StateEnabledChanged`

Fires with: (state: `Enum.HumanoidStateType`, isEnabled: `bool`)

### `Class.Humanoid.StatusAdded`

Fires with: (status: `Enum.Status`)
  [Deprecated]

### `Class.Humanoid.StatusRemoved`

Fires with: (status: `Enum.Status`)
  [Deprecated]

### `Class.Humanoid.Strafing`

Fires with: (active: `bool`)

### `Class.Humanoid.Swimming`

Fires with: (speed: `float`)

### `Class.Humanoid.Touched`

Fires with: (touchingPart: `Class.BasePart`, humanoidPart: `Class.BasePart`)
