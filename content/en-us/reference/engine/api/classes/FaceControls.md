---
title: FaceControls
type: class
superclass: Instance
---

# FaceControls

The `Class.FaceControls` object defines a set of properties for controlling
the facial expressions of a Dynamic Head.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

The `Class.FaceControls` object defines a set of properties for controlling
the facial expressions of a character head capable of animation.

The FaceControls properties are based on the Facial Action Coding System
(FACS), a comprehensive system for describing all visually discernible facial
movement based on anatomy. `Class.FaceControls` properties can only be set
between 0 and 1. Different combinations of the `Class.FaceControls` property
values create different facial expressions. Recording multiple facial
expressions over time creates facial animation.

## What is an Animatable Head?

An animatable head is a `Class.MeshPart` that implements a facial rig and is
capable of playing facial animations and triggering facial expressions. A
`Class.FaceControls` object that is a child of a head `Class.MeshPart` can
change the facial expressions of the head.

A head consists of the following three components:

- Skinned MeshPart instance for the head geometry with an internal rig that
  deforms this skinned MeshPart
- FaceControls instance that drives the internal rig when properties such as
  FaceControls.JawDrop are changed.
- Cage `Class.WrapTarget` instance for tight fitting facial accessories

In a third-party modeling tool, such as Blender or Maya, an artist can create
a joint-driven facial rig, pose the joints to match each of the individual
FACS controls, and save as an FBX. When a head `.FBX` is imported in Studio, a
facs-to-joint mapping is created. This mapping deforms the mesh geometry when
FaceControls properties are changed. The mapping and the facial rig (including
`Class.Bone` instances) are not exposed to developers and can only be accessed
through the FaceControls instance. The `Class.MeshPart` for a Dynamic Head
looks and behaves the same as a regular `Class.MeshPart` except when a
FaceControls instance is a child of the MeshPart. Editing the properties of
the FaceControls deforms the MeshPart's geometry. These properties are
available to animate in the Animation Editor.

See [Facial animation](../../../avatar/dynamic-heads/index.md) for more
information on usage and creation of an animatable head.

## Animatable Heads in the Marketplace

If you are publishing your head to the Marketplace, your head asset must
include a minimum subset of face controls. Roblox's publishing validation
rejects assets without the following required poses:

- EyesLookDown
- EyesLookLeft
- EyesLookRight
- EyesLookUp
- JawDrop
- LeftEyeClosed
- LeftLipCornerPuller
- LeftLipStretcher
- LeftLowerLipDepressor
- LeftUpperLipRaiser
- LipsTogether
- Pucker
- RightEyeClosed
- RightLipCornerPuller
- RightLipStretcher
- RightLowerLipDepressor
- RightUpperLipRaiser

See
[FACS poses reference](../../../avatar/dynamic-heads/facs-poses-reference.md)
for more information on usage and creation of an animatable head.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.FaceControls.ChinRaiser` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.ChinRaiserUpperLip` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.Corrugator` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.EyesLookDown` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.EyesLookLeft` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.EyesLookRight` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.EyesLookUp` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.FlatPucker` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.Funneler` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.JawDrop` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.JawLeft` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.JawRight` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.LeftBrowLowerer` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.LeftCheekPuff` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.LeftCheekRaiser` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.LeftDimpler` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.LeftEyeClosed` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.LeftEyeUpperLidRaiser` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.LeftInnerBrowRaiser` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.LeftLipCornerDown` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.LeftLipCornerPuller` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.LeftLipStretcher` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.LeftLowerLipDepressor` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.LeftNoseWrinkler` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.LeftOuterBrowRaiser` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.LeftUpperLipRaiser` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.LipPresser` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.LipsTogether` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.LowerLipSuck` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.MouthLeft` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.MouthRight` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.Pucker` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.RightBrowLowerer` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.RightCheekPuff` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.RightCheekRaiser` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.RightDimpler` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.RightEyeClosed` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.RightEyeUpperLidRaiser` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.RightInnerBrowRaiser` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.RightLipCornerDown` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.RightLipCornerPuller` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.RightLipStretcher` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.RightLowerLipDepressor` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.RightNoseWrinkler` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.RightOuterBrowRaiser` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.RightUpperLipRaiser` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.TongueDown` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.TongueOut` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.TongueUp` | `float` | [NotReplicated] {security: PluginSecurity} |
| `Class.FaceControls.UpperLipSuck` | `float` | [NotReplicated] {security: PluginSecurity} |

## Methods

### `Class.FaceControls:HasOverrideFACSData`

``HasOverrideFACSData()`` -> `bool`
   {security: RobloxScriptSecurity}

## Events

### `Class.FaceControls.InternalFacsOverrideChanged`

Fires with: ()
