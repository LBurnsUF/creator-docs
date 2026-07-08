---
title: CFrame
type: datatype
---

# `Datatype.CFrame`

A data type that represents both a 3D position and orientation.

## Description

The `Datatype.CFrame` data type, short for **coordinate frame**, describes a
3D position and orientation. It is made up of a **positional** component and a
**rotational** component and includes essential arithmetic operations for
working with 3D data on Roblox.

```lua
-- Create a CFrame at a certain position and Euler rotation
local cf = CFrame.new(0, 5, 0) * CFrame.fromEulerAngles(math.rad(45), 0, 0)
```

For an introduction to the `Datatype.CFrame` data type, see
[CFrames](../../../workspace/cframes.md).

#### Positional Component

The positional component is available as a `Datatype.Vector3`. In addition,
the components of a `Datatype.CFrame` object's position are also available in
the `Datatype.CFrame.X|X`, `Datatype.CFrame.Y|Y` and `Datatype.CFrame.Z|Z`
properties like a `Datatype.Vector3`.

#### Rotational Component

`Datatype.CFrame` stores 3D rotation data in a 3&times;3 **rotation matrix**.
These values are returned by the `Datatype.CFrame:GetComponents()` function
after the `x`, `y` and `z` positional values. This matrix is used internally
when doing calculations involving rotations, using **radians** as their unit
(for conversion from one to the other, use `Library.math.rad()` or
`Library.math.deg()`). For more information on how the Roblox Engine performs
rotations, see `Enum.RotationOrder`.

The table below represents the components of a `Datatype.CFrame` object's
rotation matrix and their relationship with the available vector properties
such as `Datatype.CFrame.LookVector|LookVector` and
`Datatype.CFrame.RightVector|RightVector`. Although the individual components
of the rotation matrix are rarely useful by themselves, the vector properties
which derive from them are much more useful.

<table>
  <thead>
    <tr>
      <th>XVector, RightVector</th>
      <th>YVector, UpVector</th>
      <th>ZVector, -LookVector<sup>&dagger;</sup></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>R00</td>
      <td>R01</td>
      <td>R02</td>
    </tr>
    <tr>
      <td>R10</td>
      <td>R11</td>
      <td>R12</td>
    </tr>
    <tr>
      <td>R20</td>
      <td>R21</td>
      <td>R22</td>
    </tr>
  </tbody>
</table>

<figcaption><sup>&dagger;</sup> Unlike the others,
<code>Datatype.CFrame.LookVector|LookVector</code> represents the negated
column components. The <code>Datatype.CFrame.LookVector|LookVector</code> is
useful because many <code>Class.Instance|Instances</code> such as the
<code>Class.Camera|Camera</code> and <code>Class.Attachment|Attachments</code>
treat that vector as the direction the instance is pointing.</figcaption>

## Constructors

### `CFrame.new`

Creates a blank identity `Datatype.CFrame`.

### `CFrame.new`

Returns a `Datatype.CFrame` with no rotation with the position of the
provided `Datatype.Vector3`.

**Parameters:**

- `pos`: `Vector3`

### `CFrame.new`

Returns a new `Datatype.CFrame` located at `pos` and facing towards
`lookAt`, assuming that `(0, 1, 0)` is considered "up" in world space.

This constructor overload has been replaced by `Datatype.CFrame.lookAt()`,
which accomplishes a similar goal. It remains for the sake of backward
compatibility.

At high pitch angles (around 82 degrees), you may experience numerical
instability. If this is an issue, or if you require a different "up"
vector, use `Datatype.CFrame.fromMatrix()` to more accurately construct
the `Datatype.CFrame`. Additionally, if `lookAt` is directly above `pos`
(pitch angle of 90 degrees), the "up" vector switches to the X axis.

**Parameters:**

- `pos`: `Vector3`
- `lookAt`: `Vector3`

### `CFrame.new`

Returns a `Datatype.CFrame` with a position comprised of the provided `x`, `y`, and `z` components.

**Parameters:**

- `x`: `number`
- `y`: `number`
- `z`: `number`

### `CFrame.new`

Returns a `Datatype.CFrame` from position (`x`, `y`, `z`) and
quaternion (`qX`, `qY`, `qZ`, `qW`). The quaternion is expected
to be of unit length to represent a valid rotation.
If this isn't the case, the quaternion will be normalized.

**Parameters:**

- `x`: `number`
- `y`: `number`
- `z`: `number`
- `qX`: `number`
- `qY`: `number`
- `qZ`: `number`
- `qW`: `number`

### `CFrame.new`

Creates a `Datatype.CFrame` from position (`x`, `y`, `z`) with an
orientation specified by the rotation matrix.

`[[R00 R01 R02] [R10 R11 R12] [R20 R21 R22]]`

**Parameters:**

- `x`: `number`
- `y`: `number`
- `z`: `number`
- `R00`: `number`
- `R01`: `number`
- `R02`: `number`
- `R10`: `number`
- `R11`: `number`
- `R12`: `number`
- `R20`: `number`
- `R21`: `number`
- `R22`: `number`

### `CFrame.lookAt`

Returns a new `Datatype.CFrame` with the position of `at` and facing
towards `lookAt`, optionally specifying the upward direction (`up`) with a
default of `(0, 1, 0)`.

**Parameters:**

- `at`: `Vector3`
- `lookAt`: `Vector3`
- `up`: `Vector3`

### `CFrame.lookAlong`

Returns a new `Datatype.CFrame` with the position of `at` and facing
along `direction`, optionally specifying the upward direction (`up`)
with a default of `(0, 1, 0)`.

This constructor is equivalent to `CFrame.lookAt(at, at + direction)`.

**Parameters:**

- `at`: `Vector3`
- `direction`: `Vector3`
- `up`: `Vector3`

### `CFrame.fromRotationBetweenVectors`

Returns a `Datatype.CFrame` representing the orientation needed to rotate
from the first `Datatype.Vector3` to the second, with the position set to zero.

**Parameters:**

- `from`: `Vector3` - Vector representing the "from" direction.
- `to`: `Vector3` - Vector representing the "to" direction.

### `CFrame.fromEulerAngles`

Returns a rotated `Datatype.CFrame` from angles `rx`, `ry`, and `rz` in
radians. Rotations are applied in the optional `Enum.RotationOrder` with a
default of `XYZ`, equivalent to:

```lua
CFrame.fromEulerAngles(rx, 0, 0) *  -- X
CFrame.fromEulerAngles(0, ry, 0) *  -- Y
CFrame.fromEulerAngles(0, 0, rz)    -- Z
```

**Parameters:**

- `rx`: `number`
- `ry`: `number`
- `rz`: `number`
- `order`: `RotationOrder`

### `CFrame.fromEulerAnglesXYZ`

Returns a rotated `Datatype.CFrame` from angles `rx`, `ry`, and `rz` in
radians using `Enum.RotationOrder.XYZ`, equivalent to:

```lua
CFrame.fromEulerAngles(rx, 0, 0) *  -- X
CFrame.fromEulerAngles(0, ry, 0) *  -- Y
CFrame.fromEulerAngles(0, 0, rz)    -- Z
```

**Parameters:**

- `rx`: `number`
- `ry`: `number`
- `rz`: `number`

### `CFrame.fromEulerAnglesYXZ`

Returns a rotated `Datatype.CFrame` from angles `rx`, `ry`, and `rz` in
radians using `Enum.RotationOrder.YXZ`, equivalent to:

```lua
CFrame.fromEulerAngles(0, ry, 0) *  -- Y
CFrame.fromEulerAngles(rx, 0, 0) *  -- X
CFrame.fromEulerAngles(0, 0, rz)    -- Z
```

**Parameters:**

- `rx`: `number`
- `ry`: `number`
- `rz`: `number`

### `CFrame.Angles`

Equivalent to `Datatype.CFrame.fromEulerAnglesXYZ()|fromEulerAnglesXYZ()`.

**Parameters:**

- `rx`: `number`
- `ry`: `number`
- `rz`: `number`

### `CFrame.fromOrientation`

Equivalent to `Datatype.CFrame.fromEulerAnglesYXZ()|fromEulerAnglesYXZ()`.

**Parameters:**

- `rx`: `number`
- `ry`: `number`
- `rz`: `number`

### `CFrame.fromAxisAngle`

Returns a rotated `Datatype.CFrame` from a unit `Datatype.Vector3` and a rotation in radians.

**Parameters:**

- `v`: `Vector3`
- `r`: `number`

### `CFrame.fromMatrix`

Returns a `Datatype.CFrame` from a translation and the columns of a rotation
matrix. If `vZ` is excluded, the third column is calculated as
`vX:Cross(vY).Unit`.

**Parameters:**

- `pos`: `Vector3` - The 3D position of the `Datatype.CFrame`.
- `vX`: `Vector3` - Equivalent to `Datatype.CFrame.RightVector|RightVector`.
- `vY`: `Vector3` - Equivalent to `Datatype.CFrame.UpVector|UpVector`.
- `vZ`: `Vector3` - Equivalent to -`Datatype.CFrame.LookVector|LookVector`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `CFrame.identity` | `CFrame` | An identity `Datatype.CFrame` with no translation or rotation. |
| `CFrame.Position` | `Vector3` | The 3D position of the `Datatype.CFrame`. |
| `CFrame.Rotation` | `CFrame` | A copy of the `Datatype.CFrame` with no translation. |
| `CFrame.X` | `number` | The **X** coordinate of the position. |
| `CFrame.Y` | `number` | The **Y** coordinate of the position. |
| `CFrame.Z` | `number` | The **Z** coordinate of the position. |
| `CFrame.LookVector` | `Vector3` | The forward-direction component of the `Datatype.CFrame` object's orientation, equivalent to the neg |
| `CFrame.RightVector` | `Vector3` | The right-direction component of the `Datatype.CFrame` object's orientation. |
| `CFrame.UpVector` | `Vector3` | The up-direction component of the `Datatype.CFrame` object's orientation. |
| `CFrame.XVector` | `Vector3` | Equivalent to `Datatype.CFrame.RightVector/RightVector`. |
| `CFrame.YVector` | `Vector3` | Equivalent to `Datatype.CFrame.UpVector/UpVector`. |
| `CFrame.ZVector` | `Vector3` | The Z component of the `Datatype.CFrame` object's orientation. Equivalent to the third column of the |

## Methods

### `CFrame:Inverse`

Returns the inverse of the `Datatype.CFrame`.

### `CFrame:Lerp`

Returns a `Datatype.CFrame` interpolated between itself and `goal` by the
fraction `alpha`.

**Parameters:**

- `goal`: `CFrame`
- `alpha`: `number`

### `CFrame:Orthonormalize`

Returns an orthonormalized copy of the `Datatype.CFrame`. The
`Class.BasePart.CFrame` property automatically applies orthonormalization,
but other APIs which take `Datatype.CFrame|CFrames` do not, so this method
is occasionally necessary when incrementally updating a `Datatype.CFrame`
and using it with them.

### `CFrame:ToWorldSpace`

Receives one or more `Datatype.CFrame` objects and returns them
transformed from object to world space. Equivalent to:

`CFrame * cf`

```lua
local cf = CFrame.new(5, 10, 0)

local offset = CFrame.new(0, 2, 0)

-- Output world space of offset CFrame relative to calling CFrame
print(cf:ToWorldSpace(offset))  --> 5, 12, 0, 1, 0, 0, 0, 1, 0, 0, 0, 1
```

**Parameters:**

- `...`: `Tuple<CFrame>`

### `CFrame:ToObjectSpace`

Receives one or more `Datatype.CFrame` objects and returns them
transformed from world to object space. Equivalent to:

`CFrame:Inverse() * cf`

**Parameters:**

- `...`: `Tuple<CFrame>`

### `CFrame:PointToWorldSpace`

Receives one or more `Datatype.Vector3` objects and returns them
transformed from object to world space. Equivalent to:

`CFrame * v3`

```lua
local cf = CFrame.new(5, 10, 0)

-- Output core world space of the CFrame
print(cf:PointToWorldSpace())  --> 5, 10, 0
-- Output world space of a Vector3 (0, 4, 0) relative to the CFrame (object space)
print(cf:PointToWorldSpace(Vector3.new(0, 4, 0)))  --> 5, 14, 0
```

**Parameters:**

- `...`: `Tuple<Vector3>`

### `CFrame:PointToObjectSpace`

Receives one or more `Datatype.Vector3` objects and returns them
transformed from world to object space. Equivalent to:

`CFrame:Inverse() * v3`

**Parameters:**

- `...`: `Tuple<Vector3>`

### `CFrame:VectorToWorldSpace`

Receives one or more `Datatype.Vector3` objects and returns them rotated
from object to world space. Equivalent to:

`(CFrame - CFrame.Position) * v3`

**Parameters:**

- `...`: `Tuple<Vector3>`

### `CFrame:VectorToObjectSpace`

Receives one or more `Datatype.Vector3` objects and returns them rotated
from world to object space. Equivalent to:

`(CFrame:Inverse() - CFrame:Inverse().Position) * v3`

**Parameters:**

- `...`: `Tuple<Vector3>`

### `CFrame:GetComponents`

Returns the values `x`, `y`, `z`, `R00`, `R01`, `R02`, `R10`, `R11`,
`R12`, `R20`, `R21`, and `R22`, where `x` `y` `z` represent the position
of the `Datatype.CFrame` and `R00`‑`R22` represent its 3&times;3 rotation
matrix.

### `CFrame:ToEulerAngles`

Returns approximate angles that could be used to generate the
`Datatype.CFrame` using the optional `Enum.RotationOrder`. If you don't
provide `order`, the method uses `Enum.RotationOrder.XYZ`.

**Parameters:**

- `order`: `RotationOrder`

### `CFrame:ToEulerAnglesXYZ`

Returns the approximate angles, in radians, that could be used to generate
the `Datatype.CFrame` using `Enum.RotationOrder.XYZ`.

### `CFrame:ToEulerAnglesYXZ`

Returns the approximate angles, in radians, that could be used to generate
the `Datatype.CFrame` using `Enum.RotationOrder.YXZ`.

### `CFrame:ToOrientation`

Returns the approximate angles, in radians, that could be used to generate
the `Datatype.CFrame` using `Enum.RotationOrder.YXZ`. Equivalent to
`Datatype.CFrame:ToEulerAnglesYXZ()`.

### `CFrame:ToAxisAngle`

Returns a tuple containing a unit `Datatype.Vector3` axis and a rotation
angle in radians.

### `CFrame:components`

Equivalent to `Datatype.CFrame:GetComponents()`.

### `CFrame:FuzzyEq`

Returns `true` if the other `Datatype.CFrame` is sufficiently close to
this `Datatype.CFrame` in both position and rotation. The `epsilon` value
is used to control the tolerance for this similarity; this value is
optional and should be a small positive value if provided. The similarity
for position is component-wise while rotation uses a fast approximation of
the angle difference.

**Parameters:**

- `other`: `CFrame`
- `epsilon`: `number`

### `CFrame:AngleBetween`

Returns the angle, in radians, between the orientation of one
`Datatype.CFrame` and another. This function does not take the position of
either `Datatype.CFrame` into account and only looks at the relative
orientation.

**Parameters:**

- `other`: `CFrame`

## Math Operations

| Operation | Description |
|-----------|-------------|
| `CFrame` * | Produces a new `Datatype.CFrame` representing the composition of the two `Datatype.CFrame/CFrames`. |
| `CFrame` * | Produces a `Datatype.Vector3` transformed from object to world coordinates. |
| `CFrame` + | Produces a `Datatype.CFrame` translated in world space by the `Datatype.Vector3`. |
| `CFrame` - | Produces a `Datatype.CFrame` translated in world space by the negative `Datatype.Vector3`. |

## API Usage (165 locations)

### Used as Property Type

- `Class.Accoutrement.AttachmentPoint`
- `Class.AlignOrientation.CFrame`
- `Class.AnimationConstraint.C0`
- `Class.AnimationConstraint.C1`
- `Class.AnimationConstraint.Transform`
- `Class.Animator.RootMotion`
- `Class.Attachment.CFrame`
- `Class.Attachment.WorldCFrame`
- `Class.BasePart.CFrame`
- `Class.BasePart.ExtentsCFrame`
- `Class.BasePart.PivotOffset`
- `Class.BaseWrap.CageOrigin`
- `Class.BaseWrap.CageOriginWorld`
- `Class.BaseWrap.ImportOrigin`
- `Class.BaseWrap.ImportOriginWorld`
- `Class.BodyGyro.CFrame`
- `Class.BodyGyro.cframe`
- `Class.Bone.Transform`
- `Class.Bone.TransformedCFrame`
- `Class.Bone.TransformedWorldCFrame`
- `Class.CFrameValue.Value`
- `Class.Camera.CFrame`
- `Class.Camera.CoordinateFrame`
- `Class.Camera.Focus`
- `Class.Camera.focus`
- `Class.Collaborator.CFrame`
- `Class.ControllerPartSensor.HitFrame`
- `Class.DigitsRigDescription.Index1TposeAdjustment`
- `Class.DigitsRigDescription.Index2TposeAdjustment`
- `Class.DigitsRigDescription.Index3TposeAdjustment`
- `Class.DigitsRigDescription.Middle1TposeAdjustment`
- `Class.DigitsRigDescription.Middle2TposeAdjustment`
- `Class.DigitsRigDescription.Middle3TposeAdjustment`
- `Class.DigitsRigDescription.Pinky1TposeAdjustment`
- `Class.DigitsRigDescription.Pinky2TposeAdjustment`
- `Class.DigitsRigDescription.Pinky3TposeAdjustment`
- `Class.DigitsRigDescription.Ring1TposeAdjustment`
- `Class.DigitsRigDescription.Ring2TposeAdjustment`
- `Class.DigitsRigDescription.Ring3TposeAdjustment`
- `Class.DigitsRigDescription.Thumb1TposeAdjustment`
- ...and 47 more

### Used as Parameter Type

- `Class.CFrameValue:Changed` (parameter `value`)
- `Class.CFrameValue:changed` (parameter `value`)
- `Class.Camera:Interpolate` (parameter `endFocus`)
- `Class.Camera:Interpolate` (parameter `endPos`)
- `Class.Camera:SetImageServerView` (parameter `modelCoord`)
- `Class.Camera:ZoomToExtents` (parameter `boundingBoxCFrame`)
- `Class.DigitsRigDescription:SetTposeAdjustment` (parameter `transform`)
- `Class.DragDetector:DragContinue` (parameter `viewFrame`)
- `Class.DragDetector:DragStart` (parameter `hitFrame`)
- `Class.DragDetector:DragStart` (parameter `viewFrame`)
- `Class.EditableMesh:SetBoneCFrame` (parameter `cframe`)
- `Class.EditableMesh:SetFacsBonePose` (parameter `cframe`)
- `Class.FluidForceSensor:EvaluateAsync` (parameter `cframe`)
- `Class.HumanoidRigDescription:SetTposeAdjustment` (parameter `transform`)
- `Class.Model:SetPrimaryPartCFrame` (parameter `cframe`)
- `Class.PVInstance:PivotTo` (parameter `targetCFrame`)
- `Class.PhysicsService:IkSolve` (parameter `target`)
- `Class.PhysicsService:LocalIkSolve` (parameter `target`)
- `Class.PlayerViewService:UpdateDeviceCFrame` (parameter `cframe`)
- `Class.StudioCameraService:InterpolateView` (parameter `target`)
- `Class.Terrain:DrawBufferAsync` (parameter `cframe`)
- `Class.Terrain:FillBlock` (parameter `cframe`)
- `Class.Terrain:FillCylinder` (parameter `cframe`)
- `Class.Terrain:FillWedge` (parameter `cframe`)
- `Class.Terrain:GetTerrainWireframe` (parameter `cframe`)
- `Class.Terrain:ReplaceMaterialInTransform` (parameter `cframe`)
- `Class.Terrain:ReplaceMaterialInTransformSubregion` (parameter `cframe`)
- `Class.Terrain:SetMaterialInTransform` (parameter `cframe`)
- `Class.Terrain:SetMaterialInTransformSubregion` (parameter `cframe`)
- `Class.TerrainRegion:ApplyTransform` (parameter `rotation`)
- `Class.TerrainRegion:ApplyTransformSubregion` (parameter `rotation`)
- `Class.UGCValidationService:CalculateAverageEditableCageMeshDistance` (parameter `innerTransform`)
- `Class.UGCValidationService:CalculateAverageEditableCageMeshDistance` (parameter `outerTransform`)
- `Class.UGCValidationService:CalculateEditableMeshInsideMeshPercentage` (parameter `meshQueryTransform`)
- `Class.UGCValidationService:CalculateEditableMeshModifiedCageBoundingBox` (parameter `innerTransform`)
- `Class.UGCValidationService:CalculateEditableMeshModifiedCageBoundingBox` (parameter `outerTransform`)
- `Class.UGCValidationService:CalculateEditableMeshNumModifiedCageUVsInSet` (parameter `innerTransform`)
- `Class.UGCValidationService:CalculateEditableMeshNumModifiedCageUVsInSet` (parameter `outerTransform`)
- `Class.UGCValidationService:CheckEditableMeshInCameraFrustum` (parameter `cameraWorldCF`)
- `Class.UGCValidationService:CheckEditableMeshInCameraFrustum` (parameter `handleWorldCF`)
- ...and 18 more

### Used as Return Type

- `Class.BasePart:GetRenderCFrame`
- `Class.Camera:GetRenderCFrame`
- `Class.DigitsRigDescription:GetTposeAdjustment`
- `Class.DragDetector:GetReferenceFrame`
- `Class.EditableMesh:GetBoneCFrame`
- `Class.EulerRotationCurve:GetRotationAtTime`
- `Class.HumanoidRigDescription:GetTposeAdjustment`
- `Class.IKControl:GetNodeLocalCFrame`
- `Class.IKControl:GetNodeWorldCFrame`
- `Class.IKControl:GetRawFinalTarget`
- `Class.IKControl:GetSmoothedFinalTarget`
- `Class.Model:GetModelCFrame`
- `Class.Model:GetPrimaryPartCFrame`
- `Class.PVInstance:GetPivot`
- `Class.PlayerViewService:GetDeviceCameraCFrame`
- `Class.PlayerViewService:GetDeviceCameraCFrameForSelfView`
- `Class.UGCValidationService:GetExpectedTposeRotation`
- `Class.UserInputService:GetUserCFrame`
- `Class.VRService:GetUserCFrame`
- `Class.WrapDeformer:GetDeformedCFrameAsync`
