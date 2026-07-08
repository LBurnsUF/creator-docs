---
title: Pose
type: class
superclass: PoseBase
---

# Pose

Holds the `Datatype.CFrame` applied to the `Class.Motor6D` connected to its
associated `Class.BasePart`. The part which is controlled depends on the name
of the Pose.

**Inherits from:** `Class.PoseBase` > `Class.Instance` > `Class.Object`

## Description

A Pose holds the `Datatype.CFrame` applied to the `Class.Motor6D` connected to
its associated `Class.BasePart`. The part which is controlled depends on the
name of the Pose.

Poses are the fundamental building blocks of animations and, with `Keyframes`,
make up `KeyframeSequences`.

## Poses, joints and hierarchy

Although a Pose is assigned to a `Class.BasePart` by name, the object
manipulated during animation playback is actually the `Class.Motor6D`
connected to this part. Animation rigs branch out from the model's root part
through such joints.

In a R15 character rig, the root part is the HumanoidRootPart. The LowerTorso
is connected to the HumanoidRootPart by the a motor named 'Root'. Therefore,
the `Datatype.CFrame` of a Pose named 'LowerTorso' in a `Class.Keyframe` would
be applied to the motor named 'Root', and not the LowerTorso itself.

Poses are arranged in a `Class.Keyframe` based on joint hierarchy. This means,
the Pose's `Datatype.CFrame` is applied to the motor connecting the part
associated with the pose to the part associated with the pose's parent. See
below for a visual example of the structure of Poses on a R15 character.

## Pose CFrame

The Roblox animation system applies `Class.Pose.CFrame` to the corresponding
`Class.Motor6D` by manipulating the relative transformation of the motor, the
`Class.Motor6D.Transform` property. The original `Class.JointInstance.C1|C0`
and `Class.JointInstance.C1|C1` values are not changed.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Pose.CFrame` | `Datatype.CFrame` |  |
| `Class.Pose.MaskWeight` | `float` | [NotReplicated] [Deprecated] |

## Methods

### `Class.Pose:AddSubPose`

``AddSubPose(pose: `Class.Instance`)`` -> `null`

### `Class.Pose:GetSubPoses`

``GetSubPoses()`` -> `Datatype.Instances`

### `Class.Pose:RemoveSubPose`

``RemoveSubPose(pose: `Class.Instance`)`` -> `null`
