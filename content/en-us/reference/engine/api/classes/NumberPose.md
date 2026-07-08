---
title: NumberPose
type: class
superclass: PoseBase
---

# NumberPose

Holds the value applied to a specific FACS control.

**Inherits from:** `Class.PoseBase` > `Class.Instance` > `Class.Object`

## Description

A **NumberPose** holds the value applied to a specific FACS control. The
control which is affected depends on its name.

**NumberPose** instances are the building blocks of facial animation and, with
`Class.Keyframe|Keyframes`, make up
`Class.KeyframeSequence|KeyframeSequences`.

#### NumberPoses and Facial Animation

Although a **NumberPose** is assigned to a single FACS control by name, that
control can in turn affect multiple bones of the face rig. FACS controls act
as an abstraction layer between facial muscle movements and how they are
defined in the rig.

#### NumberPose Hierarchy

Contrary to `Class.Pose` Instances, **NumberPose** instances cannot be
parented together. However, they all must be stored in a `Class.Folder` named
**FaceControls** that is a child of the **Head** `Class.Pose`.

#### NumberPose Value

The Roblox animation system applies **NumberPose** values to the corresponding
FACS controls. Because those controls only respond to values between 0 and 1,
the values calculated by the animation system are always clamped to that
range.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.NumberPose.Value` | `double` |  |
