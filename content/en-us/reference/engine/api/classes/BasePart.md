---
title: BasePart
type: class
superclass: PVInstance
tags: [NotCreatable, NotBrowsable]
---

# BasePart

The abstract base class for in-world objects that physically interact.

**Inherits from:** `Class.PVInstance` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotBrowsable]

## Description

`Class.BasePart` is an abstract base class for in-world objects that render
and are physically simulated while in the `Class.Workspace`. There are several
implementations of `Class.BasePart`, the most common being `Class.Part` and
`Class.MeshPart`. Others include `Class.WedgePart`, `Class.SpawnLocation`, and
the singleton `Class.Terrain` object. Generally, when documentation refers to
a "part," most `Class.BasePart` implementations will work and not just
`Class.Part`.

For information on how `Class.BasePart|BaseParts` are grouped into simulated
rigid bodies, see [Assemblies](../../../physics/assemblies.md).

There are many different objects that interact with `Class.BasePart` (other
than `Class.Terrain`), including:

- Several `Class.BasePart|BaseParts` may be grouped within a `Class.Model` and
  moved at the same time using `Class.PVInstance:PivotTo()`. See
  [Models](../../../parts/models.md).
- A `Class.Decal` applies a stretched image texture to the faces of a
  `Class.BasePart`, while a `Class.Texture` applies a tiled image texture to
  the faces. See [Textures and Decals](../../../parts/textures-decals.md).
- A `Class.SurfaceGui` renders `Class.GuiObject|GuiObjects` on the face of a
  part. See
  [In-Experience UI Containers](../../../ui/in-experience-containers.md).
- `Class.Attachment|Attachments` can be added to a `Class.BasePart` to specify
  `Datatype.CFrame|CFrames` relative to the part. These are often used by
  physical `Class.Constraint` objects as outlined in
  [Mechanical Constraints](../../../physics/mechanical-constraints.md) and
  [Mover Constraints](../../../physics/mover-constraints.md).
- `Class.ParticleEmitter` objects emit particles uniformly in the volume of
  the `Class.BasePart` to which they are parented. See
  [Particle Emitters](../../../effects/particle-emitters.md).
- Light objects like `Class.PointLight` emit light from the center of a
  `Class.BasePart` as illustrated in
  [Light Sources](../../../effects/light-sources.md).
- If parented to a `Class.Tool` and given the name **Handle**, a
  `Class.BasePart` can be held by characters. See
  [In-Experience Tools](../../../players/tools.md).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.BasePart.Anchored` | `bool` |  |
| `Class.BasePart.AssemblyAngularVelocity` | `Datatype.Vector3` | [NotReplicated] |
| `Class.BasePart.AssemblyCenterOfMass` | `Datatype.Vector3` | [ReadOnly] [NotReplicated] |
| `Class.BasePart.AssemblyLinearVelocity` | `Datatype.Vector3` | [NotReplicated] |
| `Class.BasePart.AssemblyMass` | `float` | [ReadOnly] [NotReplicated] |
| `Class.BasePart.AssemblyRootPart` | `Class.BasePart` | [ReadOnly] [NotReplicated] |
| `Class.BasePart.AudioCanCollide` | `bool` |  |
| `Class.BasePart.BackParamA` | `float` | [Hidden] [Deprecated] |
| `Class.BasePart.BackParamB` | `float` | [Hidden] [Deprecated] |
| `Class.BasePart.BackSurface` | `Enum.SurfaceType` |  |
| `Class.BasePart.BackSurfaceInput` | `Enum.InputType` | [Hidden] [Deprecated] |
| `Class.BasePart.BottomParamA` | `float` | [Hidden] [Deprecated] |
| `Class.BasePart.BottomParamB` | `float` | [Hidden] [Deprecated] |
| `Class.BasePart.BottomSurface` | `Enum.SurfaceType` |  |
| `Class.BasePart.BottomSurfaceInput` | `Enum.InputType` | [Hidden] [Deprecated] |
| `Class.BasePart.BrickColor` | `Datatype.BrickColor` | [NotReplicated] |
| `Class.BasePart.CFrame` | `Datatype.CFrame` |  |
| `Class.BasePart.CanCollide` | `bool` |  |
| `Class.BasePart.CanQuery` | `bool` |  |
| `Class.BasePart.CanTouch` | `bool` |  |
| `Class.BasePart.CastShadow` | `bool` |  |
| `Class.BasePart.CenterOfMass` | `Datatype.Vector3` | [ReadOnly] [NotReplicated] |
| `Class.BasePart.CollisionGroup` | `string` | [NotReplicated] |
| `Class.BasePart.CollisionGroupId` | `int` | [NotReplicated] [Deprecated] |
| `Class.BasePart.Color` | `Datatype.Color3` | [NotReplicated] |
| `Class.BasePart.CurrentPhysicalProperties` | `Datatype.PhysicalProperties` | [ReadOnly] [NotReplicated] |
| `Class.BasePart.CustomPhysicalProperties` | `Datatype.PhysicalProperties` |  |
| `Class.BasePart.Elasticity` | `float` | [Hidden] [NotReplicated] [Deprecated] |
| `Class.BasePart.EnableFluidForces` | `bool` |  |
| `Class.BasePart.ExtentsCFrame` | `Datatype.CFrame` | [ReadOnly] [NotReplicated] |
| `Class.BasePart.ExtentsSize` | `Datatype.Vector3` | [ReadOnly] [NotReplicated] |
| `Class.BasePart.Friction` | `float` | [Hidden] [NotReplicated] [Deprecated] |
| `Class.BasePart.FrontParamA` | `float` | [Hidden] [Deprecated] |
| `Class.BasePart.FrontParamB` | `float` | [Hidden] [Deprecated] |
| `Class.BasePart.FrontSurface` | `Enum.SurfaceType` |  |
| `Class.BasePart.FrontSurfaceInput` | `Enum.InputType` | [Hidden] [Deprecated] |
| `Class.BasePart.LeftParamA` | `float` | [Hidden] [Deprecated] |
| `Class.BasePart.LeftParamB` | `float` | [Hidden] [Deprecated] |
| `Class.BasePart.LeftSurface` | `Enum.SurfaceType` |  |
| `Class.BasePart.LeftSurfaceInput` | `Enum.InputType` | [Hidden] [Deprecated] |
| `Class.BasePart.LocalTransparencyModifier` | `float` | [Hidden] [NotReplicated] |
| `Class.BasePart.Locked` | `bool` |  |
| `Class.BasePart.Mass` | `float` | [ReadOnly] [NotReplicated] |
| `Class.BasePart.Massless` | `bool` |  |
| `Class.BasePart.Material` | `Enum.Material` |  |
| `Class.BasePart.MaterialVariant` | `string` | [NotReplicated] |
| `Class.BasePart.Orientation` | `Datatype.Vector3` | [Hidden] [NotReplicated] |
| `Class.BasePart.PivotOffset` | `Datatype.CFrame` |  |
| `Class.BasePart.Position` | `Datatype.Vector3` | [Hidden] [NotReplicated] |
| `Class.BasePart.ReceiveAge` | `float` | [Hidden] [ReadOnly] [NotReplicated] |
| `Class.BasePart.Reflectance` | `float` |  |
| `Class.BasePart.ResizeIncrement` | `int` | [ReadOnly] [NotReplicated] |
| `Class.BasePart.ResizeableFaces` | `Datatype.Faces` | [ReadOnly] [NotReplicated] |
| `Class.BasePart.RightParamA` | `float` | [Hidden] [Deprecated] |
| `Class.BasePart.RightParamB` | `float` | [Hidden] [Deprecated] |
| `Class.BasePart.RightSurface` | `Enum.SurfaceType` |  |
| `Class.BasePart.RightSurfaceInput` | `Enum.InputType` | [Hidden] [Deprecated] |
| `Class.BasePart.RootPriority` | `int` |  |
| `Class.BasePart.RotVelocity` | `Datatype.Vector3` | [Hidden] [Deprecated] |
| `Class.BasePart.Rotation` | `Datatype.Vector3` | [NotReplicated] |
| `Class.BasePart.Size` | `Datatype.Vector3` | [NotReplicated] |
| `Class.BasePart.SpecificGravity` | `float` | [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.BasePart.TopParamA` | `float` | [Hidden] [Deprecated] |
| `Class.BasePart.TopParamB` | `float` | [Hidden] [Deprecated] |
| `Class.BasePart.TopSurface` | `Enum.SurfaceType` |  |
| `Class.BasePart.TopSurfaceInput` | `Enum.InputType` | [Hidden] [Deprecated] |
| `Class.BasePart.Transparency` | `float` |  |
| `Class.BasePart.Velocity` | `Datatype.Vector3` | [Hidden] [Deprecated] |
| `Class.BasePart.brickColor` | `Datatype.BrickColor` | [NotReplicated] [Deprecated] |

## Methods

### `Class.BasePart:AngularAccelerationToTorque`

``AngularAccelerationToTorque(angAcceleration: `Datatype.Vector3`, angVelocity: `Datatype.Vector3`)`` -> `Datatype.Vector3`

### `Class.BasePart:ApplyAngularImpulse`

``ApplyAngularImpulse(impulse: `Datatype.Vector3`)`` -> `null`

### `Class.BasePart:ApplyImpulse`

``ApplyImpulse(impulse: `Datatype.Vector3`)`` -> `null`

### `Class.BasePart:ApplyImpulseAtPosition`

``ApplyImpulseAtPosition(impulse: `Datatype.Vector3`, position: `Datatype.Vector3`)`` -> `null`

### `Class.BasePart:BreakJoints`

``BreakJoints()`` -> `null`
  [Deprecated]

### `Class.BasePart:CanCollideWith`

``CanCollideWith(part: `Class.BasePart`)`` -> `bool`

### `Class.BasePart:CanSetNetworkOwnership`

``CanSetNetworkOwnership()`` -> `Tuple`

### `Class.BasePart:GetClosestPointOnSurface`

``GetClosestPointOnSurface(position: `Datatype.Vector3`)`` -> `Datatype.Vector3`

### `Class.BasePart:GetConnectedParts`

``GetConnectedParts(recursive: `bool`)`` -> `Datatype.Instances`

### `Class.BasePart:GetJoints`

``GetJoints()`` -> `Datatype.Instances`

### `Class.BasePart:GetMass`

``GetMass()`` -> `float`

### `Class.BasePart:GetNetworkOwner`

``GetNetworkOwner()`` -> `Class.Instance`

### `Class.BasePart:GetNetworkOwnershipAuto`

``GetNetworkOwnershipAuto()`` -> `bool`

### `Class.BasePart:GetNoCollisionConstraints`

``GetNoCollisionConstraints()`` -> `Datatype.Instances`

### `Class.BasePart:GetPhysicsCost`

``GetPhysicsCost()`` -> `float`
   {security: RobloxScriptSecurity}

### `Class.BasePart:GetRenderCFrame`

``GetRenderCFrame()`` -> `Datatype.CFrame`
  [Deprecated]

### `Class.BasePart:GetRootPart`

``GetRootPart()`` -> `Class.Instance`
  [Deprecated]

### `Class.BasePart:GetTouchingParts`

``GetTouchingParts()`` -> `Datatype.Instances`

### `Class.BasePart:GetVelocityAtPosition`

``GetVelocityAtPosition(position: `Datatype.Vector3`)`` -> `Datatype.Vector3`

### `Class.BasePart:IntersectAsync`

``IntersectAsync(parts: `Datatype.Instances`, collisionfidelity: `Enum.CollisionFidelity`, renderFidelity: `Enum.RenderFidelity`)`` -> `Class.Instance`
  [Yields]

### `Class.BasePart:IsGrounded`

``IsGrounded()`` -> `bool`

### `Class.BasePart:MakeJoints`

``MakeJoints()`` -> `null`
  [Deprecated]

### `Class.BasePart:Resize`

``Resize(normalId: `Enum.NormalId`, deltaAmount: `int`)`` -> `bool`

### `Class.BasePart:SetNetworkOwner`

``SetNetworkOwner(playerInstance: `Class.Player`)`` -> `null`

### `Class.BasePart:SetNetworkOwnershipAuto`

``SetNetworkOwnershipAuto()`` -> `null`

### `Class.BasePart:SubtractAsync`

``SubtractAsync(parts: `Datatype.Instances`, collisionfidelity: `Enum.CollisionFidelity`, renderFidelity: `Enum.RenderFidelity`)`` -> `Class.Instance`
  [Yields]

### `Class.BasePart:TorqueToAngularAcceleration`

``TorqueToAngularAcceleration(torque: `Datatype.Vector3`, angVelocity: `Datatype.Vector3`)`` -> `Datatype.Vector3`

### `Class.BasePart:UnionAsync`

``UnionAsync(parts: `Datatype.Instances`, collisionfidelity: `Enum.CollisionFidelity`, renderFidelity: `Enum.RenderFidelity`)`` -> `Class.Instance`
  [Yields]

### `Class.BasePart:breakJoints`

``breakJoints()`` -> `null`
  [Deprecated]

### `Class.BasePart:getMass`

``getMass()`` -> `float`
  [Deprecated]

### `Class.BasePart:makeJoints`

``makeJoints()`` -> `null`
  [Deprecated]

### `Class.BasePart:resize`

``resize(normalId: `Enum.NormalId`, deltaAmount: `int`)`` -> `bool`
  [Deprecated]

## Events

### `Class.BasePart.LocalSimulationTouched`

Fires with: (part: `Class.BasePart`)
  [Deprecated]

### `Class.BasePart.OutfitChanged`

Fires with: ()
  [Deprecated]

### `Class.BasePart.StoppedTouching`

Fires with: (otherPart: `Class.BasePart`)
  [Deprecated]

### `Class.BasePart.TouchEnded`

Fires with: (otherPart: `Class.BasePart`)

### `Class.BasePart.Touched`

Fires with: (otherPart: `Class.BasePart`)
