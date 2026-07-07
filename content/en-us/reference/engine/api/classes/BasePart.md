---
title: BasePart
type: class
superclass: PVInstance
tags: [NotCreatable, NotBrowsable]
---

# BasePart

**Inherits**: PVInstance > Instance > Object

**Tags**: NotCreatable, NotBrowsable

## Properties

- **Anchored**: `bool`
- **AssemblyAngularVelocity**: `Vector3` [NotReplicated]
- **AssemblyCenterOfMass**: `Vector3` [ReadOnly] [NotReplicated]
- **AssemblyLinearVelocity**: `Vector3` [NotReplicated]
- **AssemblyMass**: `float` [ReadOnly] [NotReplicated]
- **AssemblyRootPart**: `BasePart` [ReadOnly] [NotReplicated]
- **AudioCanCollide**: `bool`
- **BackParamA**: `float` [Hidden] [Deprecated]
- **BackParamB**: `float` [Hidden] [Deprecated]
- **BackSurface**: `SurfaceType`
- **BackSurfaceInput**: `InputType` [Hidden] [Deprecated]
- **BottomParamA**: `float` [Hidden] [Deprecated]
- **BottomParamB**: `float` [Hidden] [Deprecated]
- **BottomSurface**: `SurfaceType`
- **BottomSurfaceInput**: `InputType` [Hidden] [Deprecated]
- **BrickColor**: `BrickColor` [NotReplicated]
- **CFrame**: `CFrame`
- **CanCollide**: `bool`
- **CanQuery**: `bool`
- **CanTouch**: `bool`
- **CastShadow**: `bool`
- **CenterOfMass**: `Vector3` [ReadOnly] [NotReplicated]
- **CollisionGroup**: `string` [NotReplicated]
- **CollisionGroupId**: `int` [NotReplicated] [Deprecated]
- **Color**: `Color3` [NotReplicated]
- **CurrentPhysicalProperties**: `PhysicalProperties` [ReadOnly] [NotReplicated]
- **CustomPhysicalProperties**: `PhysicalProperties`
- **Elasticity**: `float` [Hidden] [NotReplicated] [Deprecated]
- **EnableFluidForces**: `bool`
- **ExtentsCFrame**: `CFrame` [ReadOnly] [NotReplicated]
- **ExtentsSize**: `Vector3` [ReadOnly] [NotReplicated]
- **Friction**: `float` [Hidden] [NotReplicated] [Deprecated]
- **FrontParamA**: `float` [Hidden] [Deprecated]
- **FrontParamB**: `float` [Hidden] [Deprecated]
- **FrontSurface**: `SurfaceType`
- **FrontSurfaceInput**: `InputType` [Hidden] [Deprecated]
- **LeftParamA**: `float` [Hidden] [Deprecated]
- **LeftParamB**: `float` [Hidden] [Deprecated]
- **LeftSurface**: `SurfaceType`
- **LeftSurfaceInput**: `InputType` [Hidden] [Deprecated]
- **LocalTransparencyModifier**: `float` [Hidden] [NotReplicated]
- **Locked**: `bool`
- **Mass**: `float` [ReadOnly] [NotReplicated]
- **Massless**: `bool`
- **Material**: `Material`
- **MaterialVariant**: `string` [NotReplicated]
- **Orientation**: `Vector3` [Hidden] [NotReplicated]
- **PivotOffset**: `CFrame`
- **Position**: `Vector3` [Hidden] [NotReplicated]
- **ReceiveAge**: `float` [Hidden] [ReadOnly] [NotReplicated]
- **Reflectance**: `float`
- **ResizeIncrement**: `int` [ReadOnly] [NotReplicated]
- **ResizeableFaces**: `Faces` [ReadOnly] [NotReplicated]
- **RightParamA**: `float` [Hidden] [Deprecated]
- **RightParamB**: `float` [Hidden] [Deprecated]
- **RightSurface**: `SurfaceType`
- **RightSurfaceInput**: `InputType` [Hidden] [Deprecated]
- **RootPriority**: `int`
- **RotVelocity**: `Vector3` [Hidden] [Deprecated]
- **Rotation**: `Vector3` [NotReplicated]
- **Size**: `Vector3` [NotReplicated]
- **SpecificGravity**: `float` [ReadOnly] [NotReplicated] [Deprecated]
- **TopParamA**: `float` [Hidden] [Deprecated]
- **TopParamB**: `float` [Hidden] [Deprecated]
- **TopSurface**: `SurfaceType`
- **TopSurfaceInput**: `InputType` [Hidden] [Deprecated]
- **Transparency**: `float`
- **Velocity**: `Vector3` [Hidden] [Deprecated]
- **brickColor**: `BrickColor` [NotReplicated] [Deprecated]

## Methods

- **AngularAccelerationToTorque**(`angAcceleration: Vector3`, `angVelocity: Vector3 = 0, 0, 0`) -> `Vector3`
- **ApplyAngularImpulse**(`impulse: Vector3`) -> `null`
- **ApplyImpulse**(`impulse: Vector3`) -> `null`
- **ApplyImpulseAtPosition**(`impulse: Vector3`, `position: Vector3`) -> `null`
- **BreakJoints**() -> `null` [Deprecated]
- **CanCollideWith**(`part: BasePart`) -> `bool`
- **CanSetNetworkOwnership**() -> `Tuple`
- **GetClosestPointOnSurface**(`position: Vector3`) -> `Vector3`
- **GetConnectedParts**(`recursive: bool = false`) -> `Instances`
- **GetJoints**() -> `Instances`
- **GetMass**() -> `float`
- **GetNetworkOwner**() -> `Instance`
- **GetNetworkOwnershipAuto**() -> `bool`
- **GetNoCollisionConstraints**() -> `Instances`
- **GetPhysicsCost**() -> `float`
- **GetRenderCFrame**() -> `CFrame` [Deprecated]
- **GetRootPart**() -> `Instance` [Deprecated]
- **GetTouchingParts**() -> `Instances`
- **GetVelocityAtPosition**(`position: Vector3`) -> `Vector3`
- **IntersectAsync**(`parts: Instances`, `collisionfidelity: CollisionFidelity = Default`, `renderFidelity: RenderFidelity = Automatic`) -> `Instance` [Yields]
- **IsGrounded**() -> `bool`
- **MakeJoints**() -> `null` [Deprecated]
- **Resize**(`normalId: NormalId`, `deltaAmount: int`) -> `bool`
- **SetNetworkOwner**(`playerInstance: Player = nil`) -> `null`
- **SetNetworkOwnershipAuto**() -> `null`
- **SubtractAsync**(`parts: Instances`, `collisionfidelity: CollisionFidelity = Default`, `renderFidelity: RenderFidelity = Automatic`) -> `Instance` [Yields]
- **TorqueToAngularAcceleration**(`torque: Vector3`, `angVelocity: Vector3 = 0, 0, 0`) -> `Vector3`
- **UnionAsync**(`parts: Instances`, `collisionfidelity: CollisionFidelity = Default`, `renderFidelity: RenderFidelity = Automatic`) -> `Instance` [Yields]
- **breakJoints**() -> `null` [Deprecated]
- **getMass**() -> `float` [Deprecated]
- **makeJoints**() -> `null` [Deprecated]
- **resize**(`normalId: NormalId`, `deltaAmount: int`) -> `bool` [Deprecated]

## Events

- **LocalSimulationTouched**(`part: BasePart`) [Deprecated]
- **OutfitChanged**() [Deprecated]
- **StoppedTouching**(`otherPart: BasePart`) [Deprecated]
- **TouchEnded**(`otherPart: BasePart`)
- **Touched**(`otherPart: BasePart`)
