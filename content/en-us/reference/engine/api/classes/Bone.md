---
title: Bone
type: class
superclass: Attachment
---

# Bone

Bones are non-rendered objects that drive the movement of one or more parts
for the purposes of animation, or creating clothing and characters.

**Inherits from:** `Class.Attachment` > `Class.Instance` > `Class.Object`

## Description

Bones are non-rendered objects that drive the movement of one or more parts
for the purposes of animation, or creating clothing and characters. Bones are
part of a `Class.Model` or `Class.MeshPart` object's skeletal **rig** that you
typically access and animate through the
[Animation Editor](../../../animation/editor.md).

Rigs are created during the modeling process in third-party software such as
Blender or Maya. After importing the rigged model into Studio, you can add the
model directly to your experience, or save and share the model as an asset.
See [Rigging](../../../art/modeling/rigging.md) for more details on creating
and using rigged models.

Note that you can parent `Class.Bone|Bones` under other `Class.Bone|Bones` and
parts. When parenting a bone to another bone, the child bone's world position
will be relative to the parent bone's position, and the hierarchy of parented
`Class.Bone` objects can change the behavior of affected parts during posing
or animation.

##### Relationship with Motor6D

To support animations with older rigs using joints, such as `Class.Motor6D`,
you can use the `Class.Bone.Transform` property in the same way as
`Class.Motor6D.Transform`. Roblox uses the offset of the bones from the
default pose to drive an animation, and bones are not replicated or
serialized.

##### Bone.CFrame

Bones inherit the `Class.Attachment.CFrame|CFrame` property of
`Class.Attachment|Attachments` which Roblox uses as the bone's reference
position. The inherited `Class.Attachment.WorldCFrame|WorldCFrame` and other
world properties return the initial un-transformed position.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Bone.Transform` | `Datatype.CFrame` | [NotReplicated] |
| `Class.Bone.TransformedCFrame` | `Datatype.CFrame` | [Hidden] [ReadOnly] [NotReplicated] |
| `Class.Bone.TransformedWorldCFrame` | `Datatype.CFrame` | [ReadOnly] [NotReplicated] |
