---
title: Vector3
type: datatype
---

# `Datatype.Vector3`

Represents a 3D value with a direction and magnitude.

## Description

The `Datatype.Vector3` data type represents a vector in 3D space, typically
used as a point in 3D space or the dimensions of a rectangular prism.
`Datatype.Vector3` supports basic component-based arithmetic operations (sum,
difference, product, and quotient) and these operations can be applied on the
left or right hand side to either another `Datatype.Vector3` or a number. It
also features methods for common vector operations, such as
`Datatype.Vector3:Cross()|Cross()` and `Datatype.Vector3:Dot()|Dot()`.

Alternatively to `Datatype.Vector3`, consider using the methods and properties
of the `Library.vector` library.

Some example usages of `Datatype.Vector3` are the
`Class.BasePart.Position|Position`, `Class.BasePart.Rotation|Rotation`, and
`Class.BasePart.Size|Size` of parts, for example:

```lua
local Workspace = game:GetService("Workspace")

local part = Workspace.Part
part.Position = part.Position + Vector3.new(5, 2, 10) -- Move part by (5, 2, 10)
```

`Datatype.Vector3` is also commonly used when constructing more complex 3D
data types such as `Datatype.CFrame`. Many of these data types' methods will
use a `Datatype.Vector3` within their parameters, such as
`Datatype.CFrame:PointToObjectSpace()`.

## Constructors

### `Vector3.new`

Returns a new `Datatype.Vector3` using the given `x`, `y`, and `z` components.

**Parameters:**

- `x`: `number`
- `y`: `number`
- `z`: `number`

### `Vector3.FromNormalId`

Returns a new `Datatype.Vector3` in the given direction.

**Parameters:**

- `normal`: `NormalId`

### `Vector3.FromAxis`

Returns a new `Datatype.Vector3` for the given axis.

**Parameters:**

- `axis`: `Axis`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Vector3.zero` | `Vector3` | A `Datatype.Vector3` with a magnitude of `0`. |
| `Vector3.one` | `Vector3` | A `Datatype.Vector3` with a value of `1` on every axis. |
| `Vector3.xAxis` | `Vector3` | A `Datatype.Vector3` with a value of `1` on the **X** axis. |
| `Vector3.yAxis` | `Vector3` | A `Datatype.Vector3` with a value of `1 `on the **Y** axis. |
| `Vector3.zAxis` | `Vector3` | A `Datatype.Vector3` with a value of `1` on the **Z** axis. |
| `Vector3.X` | `number` | The **X** coordinate of the `Datatype.Vector3`. |
| `Vector3.Y` | `number` | The **Y** coordinate of the `Datatype.Vector3`. |
| `Vector3.Z` | `number` | The **Z** coordinate of the `Datatype.Vector3`. |
| `Vector3.Magnitude` | `number` | The length of the `Datatype.Vector3`. |
| `Vector3.Unit` | `Vector3` | A normalized copy of the `Datatype.Vector3` - one that has the same direction as the original but a  |

## Methods

### `Vector3:Abs`

Returns a new vector from the absolute values of the original's
components. For example, a vector of `(-2, 4, -6)` returns a vector of
`(2, 4, 6)`.

### `Vector3:Ceil`

Returns a new vector from the ceiling of the original's components. For
example, a vector of `(-2.6, 5.1, 8.8)` returns a vector of `(-2, 6, 9)`.

### `Vector3:Floor`

Returns a new vector from the floor of the original's components. For
example, a vector of `(-2.6, 5.1, 8.8)` returns a vector of `(-3, 5, 8)`.

### `Vector3:Sign`

Returns a new vector from the sign (-1, 0, or 1) of the original's
components. For example, a vector of `(-2.6, 5.1, 0)` returns a vector of
`(-1, 1, 0)`.

### `Vector3:Cross`

Returns the cross product of the two vectors.

**Parameters:**

- `other`: `Vector3`

### `Vector3:Angle`

Returns the angle in radians between the two vectors. If you provide an
axis, it determines the sign of the angle.

**Parameters:**

- `other`: `Vector3`
- `axis`: `Vector3`

### `Vector3:Dot`

Returns a scalar dot product of the two vectors.

**Parameters:**

- `other`: `Vector3`

### `Vector3:FuzzyEq`

Returns `true` if the difference between the squared magnitude of the two
vectors is within `epsilon`. `epsilon` is scaled relative to the
magnitude, rather than an absolute epsilon.

**Parameters:**

- `other`: `Vector3`
- `epsilon`: `number`

### `Vector3:Lerp`

Returns a `Datatype.Vector3` linearly interpolated between this
`Datatype.Vector3` and the given `goal` `Datatype.Vector3` by the fraction
`alpha`. Note that `alpha` is **not** limited to the range `[0, 1]`.

**Parameters:**

- `goal`: `Vector3`
- `alpha`: `number`

### `Vector3:Max`

Returns a `Datatype.Vector3` with each component as the highest among the
respective components of both provided `Datatype.Vector3` objects.

```lua
local a = Vector3.new(1, 2, 1)
local b = Vector3.new(2, 1, 2)

print(a:Max(b))  --> Vector3.new(2, 2, 2)
```

**Parameters:**

- `vector`: `Vector3`

### `Vector3:Min`

Returns a `Datatype.Vector3` with each component as the lowest among the
respective components of both provided `Datatype.Vector3` objects.

```lua
local a = Vector3.new(1, 2, 1)
local b = Vector3.new(2, 1, 2)

print(a:Min(b))  --> Vector3.new(1, 1, 1)
```

**Parameters:**

- `vector`: `Vector3`

## Math Operations

| Operation | Description |
|-----------|-------------|
| `Vector3` + | Produces a `Datatype.Vector3` by adding each component of the first vector to the corresponding comp |
| `Vector3` - | Produces a `Datatype.Vector3` by subtracting each component of the second vector from the correspond |
| `Vector3` * | Produces a `Datatype.Vector3` by multiplying each component of the first vector by the corresponding |
| `Vector3` / | Produces a `Datatype.Vector3` by dividing each component of the first vector by the corresponding co |
| `Vector3` // | Produces a `Datatype.Vector3` by **floor dividing** each component of the first vector by the corres |
| `Vector3` * | Produces a `Datatype.Vector3` by multiplying each component of the provided vector by the number. |
| `Vector3` / | Produces a `Datatype.Vector3` by dividing each component of the provided vector by the number. |
| `Vector3` // | Produces a `Datatype.Vector3` by **floor dividing** each component of the provided vector by the num |

## API Usage (331 locations)

### Used as Property Type

- `Class.AccessoryDescription.Position`
- `Class.AccessoryDescription.Rotation`
- `Class.AccessoryDescription.Scale`
- `Class.Accoutrement.AttachmentForward`
- `Class.Accoutrement.AttachmentPos`
- `Class.Accoutrement.AttachmentRight`
- `Class.Accoutrement.AttachmentUp`
- `Class.AirController.LinearImpulse`
- `Class.AlignOrientation.LookAtPosition`
- `Class.AlignOrientation.PrimaryAxis`
- `Class.AlignOrientation.SecondaryAxis`
- `Class.AlignPosition.MaxAxesForce`
- `Class.AlignPosition.Position`
- `Class.AngularVelocity.AngularVelocity`
- `Class.AtmosphereSensor.RelativeWindVelocity`
- `Class.Attachment.Axis`
- `Class.Attachment.Orientation`
- `Class.Attachment.Position`
- `Class.Attachment.Rotation`
- `Class.Attachment.SecondaryAxis`
- `Class.Attachment.WorldAxis`
- `Class.Attachment.WorldOrientation`
- `Class.Attachment.WorldPosition`
- `Class.Attachment.WorldRotation`
- `Class.Attachment.WorldSecondaryAxis`
- `Class.AvatarAccessoryRules.LimitBounds`
- `Class.AvatarClothingRules.LimitBounds`
- `Class.AvatarCollisionRules.SingleColliderSize`
- `Class.BasePart.AssemblyAngularVelocity`
- `Class.BasePart.AssemblyCenterOfMass`
- `Class.BasePart.AssemblyLinearVelocity`
- `Class.BasePart.CenterOfMass`
- `Class.BasePart.ExtentsSize`
- `Class.BasePart.Orientation`
- `Class.BasePart.Position`
- `Class.BasePart.RotVelocity`
- `Class.BasePart.Rotation`
- `Class.BasePart.Size`
- `Class.BasePart.Velocity`
- `Class.BillboardGui.ExtentsOffset`
- ...and 143 more

### Used as Parameter Type

- `Class.Attachment:SetAxis` (parameter `axis`)
- `Class.Attachment:SetSecondaryAxis` (parameter `axis`)
- `Class.BasePart:AngularAccelerationToTorque` (parameter `angAcceleration`)
- `Class.BasePart:AngularAccelerationToTorque` (parameter `angVelocity`)
- `Class.BasePart:ApplyAngularImpulse` (parameter `impulse`)
- `Class.BasePart:ApplyImpulse` (parameter `impulse`)
- `Class.BasePart:ApplyImpulseAtPosition` (parameter `impulse`)
- `Class.BasePart:ApplyImpulseAtPosition` (parameter `position`)
- `Class.BasePart:GetClosestPointOnSurface` (parameter `position`)
- `Class.BasePart:GetVelocityAtPosition` (parameter `position`)
- `Class.BasePart:TorqueToAngularAcceleration` (parameter `angVelocity`)
- `Class.BasePart:TorqueToAngularAcceleration` (parameter `torque`)
- `Class.Camera:WorldToScreenPoint` (parameter `worldPoint`)
- `Class.Camera:WorldToViewportPoint` (parameter `worldPoint`)
- `Class.Camera:ZoomToExtents` (parameter `boundingBoxSize`)
- `Class.DigitsRigDescription:SetFingerControl` (parameter `control`)
- `Class.DigitsRigDescription:SetFingerTip` (parameter `point`)
- `Class.Dragger:MouseDown` (parameter `pointOnMousePart`)
- `Class.EditableMesh:AddNormal` (parameter `normal`)
- `Class.EditableMesh:AddVertex` (parameter `p`)
- `Class.EditableMesh:FindClosestPointOnSurface` (parameter `point`)
- `Class.EditableMesh:FindClosestVertex` (parameter `toThisPoint`)
- `Class.EditableMesh:FindVerticesWithinSphere` (parameter `center`)
- `Class.EditableMesh:RaycastLocal` (parameter `direction`)
- `Class.EditableMesh:RaycastLocal` (parameter `origin`)
- `Class.EditableMesh:SetNormal` (parameter `normal`)
- `Class.EditableMesh:SetPosition` (parameter `p`)
- `Class.FluidForceSensor:EvaluateAsync` (parameter `angularVelocity`)
- `Class.FluidForceSensor:EvaluateAsync` (parameter `linearVelocity`)
- `Class.GuiService:GetClosestDialogToPosition` (parameter `position`)
- `Class.GuiService:GetClosestVisibleDialogToPosition` (parameter `position`)
- `Class.Humanoid:Move` (parameter `moveDirection`)
- `Class.Humanoid:MoveTo` (parameter `location`)
- `Class.HumanoidRigDescription:SetJointRangeMax` (parameter `rangeMax`)
- `Class.HumanoidRigDescription:SetJointRangeMin` (parameter `rangeMin`)
- `Class.Model:MoveTo` (parameter `position`)
- `Class.Model:TranslateBy` (parameter `delta`)
- `Class.Model:move` (parameter `location`)
- `Class.Model:moveTo` (parameter `location`)
- `Class.Noise:SampleDirectional` (parameter `direction`)
- ...and 71 more

### Used as Return Type

- `Class.Attachment:GetAxis`
- `Class.Attachment:GetSecondaryAxis`
- `Class.BasePart:AngularAccelerationToTorque`
- `Class.BasePart:GetClosestPointOnSurface`
- `Class.BasePart:GetVelocityAtPosition`
- `Class.BasePart:TorqueToAngularAcceleration`
- `Class.BaseWrap:GetCageOffset`
- `Class.BodyPosition:GetLastForce`
- `Class.BodyPosition:lastForce`
- `Class.BodyVelocity:GetLastForce`
- `Class.BodyVelocity:lastForce`
- `Class.Constraint:GetDebugAppliedForce`
- `Class.Constraint:GetDebugAppliedTorque`
- `Class.DigitsRigDescription:GetFingerControl`
- `Class.DigitsRigDescription:GetFingerTip`
- `Class.EditableMesh:GetCenter`
- `Class.EditableMesh:GetNormal`
- `Class.EditableMesh:GetPosition`
- `Class.EditableMesh:GetSize`
- `Class.Humanoid:ComputeOriginalSizeForPart`
- `Class.Humanoid:GetAccessoryHandleScale`
- `Class.Humanoid:GetMoveVelocity`
- `Class.Humanoid:GetRelativeVelocityAtFloor`
- `Class.HumanoidRigDescription:GetJointRangeMax`
- `Class.HumanoidRigDescription:GetJointRangeMin`
- `Class.Lighting:GetMoonDirection`
- `Class.Lighting:GetSunDirection`
- `Class.Model:GetExtentsSize`
- `Class.Model:GetModelSize`
- `Class.Terrain:CellCenterToWorld`
- `Class.Terrain:CellCornerToWorld`
- `Class.Terrain:WorldToCell`
- `Class.Terrain:WorldToCellPreferEmpty`
- `Class.Terrain:WorldToCellPreferSolid`
- `Class.UGCValidationService:GetLayeredClothingPostDeformationSize`
- `Class.VoxelBuffer:GetSizeInVoxels`
- `Class.WorkspaceAnnotation:GetAbsolutePosition`
