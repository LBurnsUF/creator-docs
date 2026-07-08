---
title: HumanoidRigDescription
type: class
superclass: Instance
---

# HumanoidRigDescription

Stores the joint mapping, T-pose, and per-joint properties for a 22-joint
bipedal character rig. Joints may be `Class.AnimationConstraint`,
`Class.Motor6D`, or `Class.Bone` instances.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

Stores the joint mapping, reference T-pose and per-joint properties for a
bipedal `Humanoid` character rig. Each of the 22 joints in the rig hierarchy
can reference an `Instance` (typically a `Motor6D`, `AnimationConstraint` or
`Bone`), define a T-pose adjustment transform, rotation range limits, and
carry a size for volumetric visualization and retargeting. For an example
Blender and Maya rig hierarchy with all optional joints, see
[Character specifications - Higher-fidelity rigs](../../../avatar/character-bodies/specifications.md#higher-fidelity-rigs).

Use `AutoRig` to automatically populate joint references from a character
model, or assign joints individually. Supports both R6 (6-joint) and R15
(15-joint) rig subsets in addition to the full 22-joint standard set, as well
as rigs with more than 22 joints by mapping the key subset of joints.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.HumanoidRigDescription.Chest` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.ChestRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.ChestRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.ChestSize` | `float` |  |
| `Class.HumanoidRigDescription.ChestTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.HeadBase` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.HeadBaseRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.HeadBaseRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.HeadBaseSize` | `float` |  |
| `Class.HumanoidRigDescription.HeadBaseTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.LeftAnkle` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.LeftAnkleRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.LeftAnkleRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.LeftAnkleSize` | `float` |  |
| `Class.HumanoidRigDescription.LeftAnkleTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.LeftClavicle` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.LeftClavicleRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.LeftClavicleRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.LeftClavicleSize` | `float` |  |
| `Class.HumanoidRigDescription.LeftClavicleTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.LeftElbow` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.LeftElbowRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.LeftElbowRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.LeftElbowSize` | `float` |  |
| `Class.HumanoidRigDescription.LeftElbowTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.LeftHip` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.LeftHipRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.LeftHipRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.LeftHipSize` | `float` |  |
| `Class.HumanoidRigDescription.LeftHipTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.LeftKnee` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.LeftKneeRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.LeftKneeRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.LeftKneeSize` | `float` |  |
| `Class.HumanoidRigDescription.LeftKneeTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.LeftShoulder` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.LeftShoulderRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.LeftShoulderRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.LeftShoulderSize` | `float` |  |
| `Class.HumanoidRigDescription.LeftShoulderTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.LeftToeBase` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.LeftToeBaseRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.LeftToeBaseRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.LeftToeBaseSize` | `float` |  |
| `Class.HumanoidRigDescription.LeftToeBaseTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.LeftWrist` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.LeftWristRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.LeftWristRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.LeftWristSize` | `float` |  |
| `Class.HumanoidRigDescription.LeftWristTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.Neck` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.NeckRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.NeckRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.NeckSize` | `float` |  |
| `Class.HumanoidRigDescription.NeckTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.OriginOffset` | `Datatype.CFrame` |  {security: RobloxScriptSecurity} |
| `Class.HumanoidRigDescription.RightAnkle` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.RightAnkleRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.RightAnkleRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.RightAnkleSize` | `float` |  |
| `Class.HumanoidRigDescription.RightAnkleTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.RightClavicle` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.RightClavicleRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.RightClavicleRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.RightClavicleSize` | `float` |  |
| `Class.HumanoidRigDescription.RightClavicleTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.RightElbow` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.RightElbowRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.RightElbowRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.RightElbowSize` | `float` |  |
| `Class.HumanoidRigDescription.RightElbowTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.RightHip` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.RightHipRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.RightHipRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.RightHipSize` | `float` |  |
| `Class.HumanoidRigDescription.RightHipTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.RightKnee` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.RightKneeRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.RightKneeRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.RightKneeSize` | `float` |  |
| `Class.HumanoidRigDescription.RightKneeTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.RightShoulder` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.RightShoulderRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.RightShoulderRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.RightShoulderSize` | `float` |  |
| `Class.HumanoidRigDescription.RightShoulderTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.RightToeBase` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.RightToeBaseRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.RightToeBaseRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.RightToeBaseSize` | `float` |  |
| `Class.HumanoidRigDescription.RightToeBaseTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.RightWrist` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.RightWristRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.RightWristRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.RightWristSize` | `float` |  |
| `Class.HumanoidRigDescription.RightWristTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.Root` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.RootRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.RootRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.RootSize` | `float` |  |
| `Class.HumanoidRigDescription.RootTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.Spine` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.SpineRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.SpineRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.SpineSize` | `float` |  |
| `Class.HumanoidRigDescription.SpineTposeAdjustment` | `Datatype.CFrame` |  |
| `Class.HumanoidRigDescription.Waist` | `Class.Instance` |  |
| `Class.HumanoidRigDescription.WaistRangeMax` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.WaistRangeMin` | `Datatype.Vector3` |  |
| `Class.HumanoidRigDescription.WaistSize` | `float` |  |
| `Class.HumanoidRigDescription.WaistTposeAdjustment` | `Datatype.CFrame` |  |

## Methods

### `Class.HumanoidRigDescription:AutoRig`

``AutoRig(character: `Class.Instance`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.HumanoidRigDescription:GetContainedJointLabels`

``GetContainedJointLabels(bodyMeshPartName: `string`)`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.HumanoidRigDescription:GetJoint`

``GetJoint(label: `Enum.RigLabel`)`` -> `Class.Instance`
   {security: RobloxScriptSecurity}

### `Class.HumanoidRigDescription:GetJointFromName`

``GetJointFromName(name: `string`)`` -> `Class.Instance`

### `Class.HumanoidRigDescription:GetJointLabels`

``GetJointLabels()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.HumanoidRigDescription:GetJointNames`

``GetJointNames()`` -> `Array`

### `Class.HumanoidRigDescription:GetJointRangeMax`

``GetJointRangeMax(rigLabel: `Enum.RigLabel`)`` -> `Datatype.Vector3`
   {security: RobloxScriptSecurity}

### `Class.HumanoidRigDescription:GetJointRangeMin`

``GetJointRangeMin(rigLabel: `Enum.RigLabel`)`` -> `Datatype.Vector3`
   {security: RobloxScriptSecurity}

### `Class.HumanoidRigDescription:GetJointSize`

``GetJointSize(label: `Enum.RigLabel`)`` -> `float`
   {security: RobloxScriptSecurity}

### `Class.HumanoidRigDescription:GetR15JointLabels`

``GetR15JointLabels()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.HumanoidRigDescription:GetR15JointNames`

``GetR15JointNames()`` -> `Array`

### `Class.HumanoidRigDescription:GetR6JointLabels`

``GetR6JointLabels()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.HumanoidRigDescription:GetR6JointNames`

``GetR6JointNames()`` -> `Array`

### `Class.HumanoidRigDescription:GetTposeAdjustment`

``GetTposeAdjustment(label: `Enum.RigLabel`)`` -> `Datatype.CFrame`
   {security: RobloxScriptSecurity}

### `Class.HumanoidRigDescription:SetJoint`

``SetJoint(label: `Enum.RigLabel`, joint: `Class.Instance`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.HumanoidRigDescription:SetJointRangeMax`

``SetJointRangeMax(rigLabel: `Enum.RigLabel`, rangeMax: `Datatype.Vector3`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.HumanoidRigDescription:SetJointRangeMin`

``SetJointRangeMin(rigLabel: `Enum.RigLabel`, rangeMin: `Datatype.Vector3`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.HumanoidRigDescription:SetJointSize`

``SetJointSize(label: `Enum.RigLabel`, size: `float`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.HumanoidRigDescription:SetTposeAdjustment`

``SetTposeAdjustment(label: `Enum.RigLabel`, transform: `Datatype.CFrame`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.HumanoidRigDescription:ShowVolumes`

``ShowVolumes(show: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}
