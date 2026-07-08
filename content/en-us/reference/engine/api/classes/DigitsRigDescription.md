---
title: DigitsRigDescription
type: class
superclass: Instance
---

# DigitsRigDescription

Maps the 15 phalanx joints of one hand (5 fingers, 3 joints each) and exposes
forward- and inverse-kinematics helpers for controlling finger poses at
runtime.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

Enables interoperability of animations across hand rigs and drives the hand
finger solver. Each `DigitsRigDescription` maps the 15 phalanx joints of one
hand (5 fingers with 3 joints each) to engine instances, stores their T-pose
adjustments, and exposes forward- and inverse-kinematics helpers for
controlling finger poses at runtime.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.DigitsRigDescription.Index1` | `Class.Instance` |  |
| `Class.DigitsRigDescription.Index1TposeAdjustment` | `Datatype.CFrame` |  |
| `Class.DigitsRigDescription.Index2` | `Class.Instance` |  |
| `Class.DigitsRigDescription.Index2TposeAdjustment` | `Datatype.CFrame` |  |
| `Class.DigitsRigDescription.Index3` | `Class.Instance` |  |
| `Class.DigitsRigDescription.Index3TposeAdjustment` | `Datatype.CFrame` |  |
| `Class.DigitsRigDescription.IndexRange` | `Datatype.Vector3` |  |
| `Class.DigitsRigDescription.IndexSize` | `float` |  |
| `Class.DigitsRigDescription.Middle1` | `Class.Instance` |  |
| `Class.DigitsRigDescription.Middle1TposeAdjustment` | `Datatype.CFrame` |  |
| `Class.DigitsRigDescription.Middle2` | `Class.Instance` |  |
| `Class.DigitsRigDescription.Middle2TposeAdjustment` | `Datatype.CFrame` |  |
| `Class.DigitsRigDescription.Middle3` | `Class.Instance` |  |
| `Class.DigitsRigDescription.Middle3TposeAdjustment` | `Datatype.CFrame` |  |
| `Class.DigitsRigDescription.MiddleRange` | `Datatype.Vector3` |  |
| `Class.DigitsRigDescription.MiddleSize` | `float` |  |
| `Class.DigitsRigDescription.Pinky1` | `Class.Instance` |  |
| `Class.DigitsRigDescription.Pinky1TposeAdjustment` | `Datatype.CFrame` |  |
| `Class.DigitsRigDescription.Pinky2` | `Class.Instance` |  |
| `Class.DigitsRigDescription.Pinky2TposeAdjustment` | `Datatype.CFrame` |  |
| `Class.DigitsRigDescription.Pinky3` | `Class.Instance` |  |
| `Class.DigitsRigDescription.Pinky3TposeAdjustment` | `Datatype.CFrame` |  |
| `Class.DigitsRigDescription.PinkyRange` | `Datatype.Vector3` |  |
| `Class.DigitsRigDescription.PinkySize` | `float` |  |
| `Class.DigitsRigDescription.Ring1` | `Class.Instance` |  |
| `Class.DigitsRigDescription.Ring1TposeAdjustment` | `Datatype.CFrame` |  |
| `Class.DigitsRigDescription.Ring2` | `Class.Instance` |  |
| `Class.DigitsRigDescription.Ring2TposeAdjustment` | `Datatype.CFrame` |  |
| `Class.DigitsRigDescription.Ring3` | `Class.Instance` |  |
| `Class.DigitsRigDescription.Ring3TposeAdjustment` | `Datatype.CFrame` |  |
| `Class.DigitsRigDescription.RingRange` | `Datatype.Vector3` |  |
| `Class.DigitsRigDescription.RingSize` | `float` |  |
| `Class.DigitsRigDescription.Side` | `Enum.DigitsRigDescriptionSide` |  |
| `Class.DigitsRigDescription.Thumb1` | `Class.Instance` |  |
| `Class.DigitsRigDescription.Thumb1TposeAdjustment` | `Datatype.CFrame` |  |
| `Class.DigitsRigDescription.Thumb2` | `Class.Instance` |  |
| `Class.DigitsRigDescription.Thumb2TposeAdjustment` | `Datatype.CFrame` |  |
| `Class.DigitsRigDescription.Thumb3` | `Class.Instance` |  |
| `Class.DigitsRigDescription.Thumb3TposeAdjustment` | `Datatype.CFrame` |  |
| `Class.DigitsRigDescription.ThumbRange` | `Datatype.Vector3` |  |
| `Class.DigitsRigDescription.ThumbSize` | `float` |  |

## Methods

### `Class.DigitsRigDescription:GetFingerControl`

``GetFingerControl(fingerIndex: `int`)`` -> `Datatype.Vector3`

### `Class.DigitsRigDescription:GetFingerTip`

``GetFingerTip(fingerIndex: `int`)`` -> `Datatype.Vector3`

### `Class.DigitsRigDescription:GetJoint`

``GetJoint(label: `Enum.RigLabel`)`` -> `Class.Instance`
   {security: RobloxScriptSecurity}

### `Class.DigitsRigDescription:GetJointLabels`

``GetJointLabels()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.DigitsRigDescription:GetTposeAdjustment`

``GetTposeAdjustment(label: `Enum.RigLabel`)`` -> `Datatype.CFrame`
   {security: RobloxScriptSecurity}

### `Class.DigitsRigDescription:SetFingerControl`

``SetFingerControl(fingerIndex: `int`, control: `Datatype.Vector3`)`` -> `null`

### `Class.DigitsRigDescription:SetFingerTip`

``SetFingerTip(fingerIndex: `int`, point: `Datatype.Vector3`)`` -> `null`

### `Class.DigitsRigDescription:SetJoint`

``SetJoint(label: `Enum.RigLabel`, joint: `Class.Instance`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.DigitsRigDescription:SetTposeAdjustment`

``SetTposeAdjustment(label: `Enum.RigLabel`, transform: `Datatype.CFrame`)`` -> `null`
   {security: RobloxScriptSecurity}
