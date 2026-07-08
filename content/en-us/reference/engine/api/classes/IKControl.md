---
title: IKControl
type: class
superclass: Instance
---

# IKControl

Specifies a control to generate a procedural animation pose using Inverse
Kinematics.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

**IKControl** instances generate procedural animation poses using Inverse
Kinematics (IK). They allow you to make characters respond realistically to
their environment.

For example, you can make a character place its hand on a door handle exactly,
and the character will do so independently of its position.
`Class.IKControl|IKControls` provide the advantage of needing to create much
fewer animations for your game while giving your experience a more realistic
and polished feel.

`Class.IKControl|IKControls` must be a child of a `Class.Humanoid` or
`Class.AnimationController` with an `Class.Animator` and have all of their
required properties set properly, otherwise they don't have any effect. The
required properties are `Class.IKControl.Type|Type`,
`Class.IKControl.EndEffector|EndEffector`, `Class.IKControl.Target|Target`,
`Class.IKControl.ChainRoot|ChainRoot`. As soon as those are set, the
`Class.IKControl` modifies the pose of your character as you specify. The
following code sample demonstrates how to set up your first `Class.IKControl`
and get started with creating more realistic animations for your game.

You can use `Class.IKControl|IKControls` to make a character:

- Rotate its head and torso to look at a point of interest in the world.
- Modify its feet positions to respond to dynamic terrain. Adjust its legs and
  feet to place them accordingly on terrain with rocks and slopes.
- Hold a gun and place its hands appropriately on the grip without needing to
  create animations for each gun in the game.
- Aim at a point in the world, so that the tip of the gun point exactly at
  what you want to shoot. Especially useful in third person shooters.
- Place its hands on the steering wheel of a car and follow it when it
  rotates.
- Much more!

`Class.IKControl` will override the animation for all the parts between the
`Class.IKControl.ChainRoot|ChainRoot` and the
`Class.IKControl.EndEffector|EndEffector`. You can enable/disable it using
`Class.IKControl.Enabled|Enabled` or change how much they have an effect over
the underlying animation using the `Class.IKControl.Weight|Weight`. Be
careful: if you do not set up your `Class.IKControl|IKControls` correctly, you
might generate bad and unrealistic poses!

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.IKControl.ChainRoot` | `Class.Instance` |  |
| `Class.IKControl.Enabled` | `bool` |  |
| `Class.IKControl.EndEffector` | `Class.Instance` |  |
| `Class.IKControl.EndEffectorOffset` | `Datatype.CFrame` |  |
| `Class.IKControl.Offset` | `Datatype.CFrame` |  |
| `Class.IKControl.Pole` | `Class.Instance` |  |
| `Class.IKControl.Priority` | `int` |  |
| `Class.IKControl.SmoothTime` | `float` |  |
| `Class.IKControl.Target` | `Class.Instance` |  |
| `Class.IKControl.Type` | `Enum.IKControlType` |  |
| `Class.IKControl.Weight` | `float` |  |

## Methods

### `Class.IKControl:GetChainCount`

``GetChainCount()`` -> `int`

### `Class.IKControl:GetChainLength`

``GetChainLength()`` -> `float`

### `Class.IKControl:GetNodeLocalCFrame`

``GetNodeLocalCFrame(index: `int`)`` -> `Datatype.CFrame`

### `Class.IKControl:GetNodeWorldCFrame`

``GetNodeWorldCFrame(index: `int`)`` -> `Datatype.CFrame`

### `Class.IKControl:GetRawFinalTarget`

``GetRawFinalTarget()`` -> `Datatype.CFrame`

### `Class.IKControl:GetSmoothedFinalTarget`

``GetSmoothedFinalTarget()`` -> `Datatype.CFrame`

### `Class.IKControl:Solve`

``Solve()`` -> `null`
   {security: RobloxScriptSecurity}
