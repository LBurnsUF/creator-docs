---
title: DigitsRigDescription
type: class
superclass: Instance
---

# DigitsRigDescription

**Inherits**: Instance > Object

## Properties

- **Index1**: `Instance`
- **Index1TposeAdjustment**: `CFrame`
- **Index2**: `Instance`
- **Index2TposeAdjustment**: `CFrame`
- **Index3**: `Instance`
- **Index3TposeAdjustment**: `CFrame`
- **IndexRange**: `Vector3`
- **IndexSize**: `float`
- **Middle1**: `Instance`
- **Middle1TposeAdjustment**: `CFrame`
- **Middle2**: `Instance`
- **Middle2TposeAdjustment**: `CFrame`
- **Middle3**: `Instance`
- **Middle3TposeAdjustment**: `CFrame`
- **MiddleRange**: `Vector3`
- **MiddleSize**: `float`
- **Pinky1**: `Instance`
- **Pinky1TposeAdjustment**: `CFrame`
- **Pinky2**: `Instance`
- **Pinky2TposeAdjustment**: `CFrame`
- **Pinky3**: `Instance`
- **Pinky3TposeAdjustment**: `CFrame`
- **PinkyRange**: `Vector3`
- **PinkySize**: `float`
- **Ring1**: `Instance`
- **Ring1TposeAdjustment**: `CFrame`
- **Ring2**: `Instance`
- **Ring2TposeAdjustment**: `CFrame`
- **Ring3**: `Instance`
- **Ring3TposeAdjustment**: `CFrame`
- **RingRange**: `Vector3`
- **RingSize**: `float`
- **Side**: `DigitsRigDescriptionSide`
- **Thumb1**: `Instance`
- **Thumb1TposeAdjustment**: `CFrame`
- **Thumb2**: `Instance`
- **Thumb2TposeAdjustment**: `CFrame`
- **Thumb3**: `Instance`
- **Thumb3TposeAdjustment**: `CFrame`
- **ThumbRange**: `Vector3`
- **ThumbSize**: `float`

## Methods

- **GetFingerControl**(`fingerIndex: int`) -> `Vector3`
- **GetFingerTip**(`fingerIndex: int`) -> `Vector3`
- **GetJoint**(`label: RigLabel`) -> `Instance`
- **GetJointLabels**() -> `Array`
- **GetTposeAdjustment**(`label: RigLabel`) -> `CFrame`
- **SetFingerControl**(`fingerIndex: int`, `control: Vector3`) -> `null`
- **SetFingerTip**(`fingerIndex: int`, `point: Vector3`) -> `null`
- **SetJoint**(`label: RigLabel`, `joint: Instance`) -> `null`
- **SetTposeAdjustment**(`label: RigLabel`, `transform: CFrame`) -> `null`
