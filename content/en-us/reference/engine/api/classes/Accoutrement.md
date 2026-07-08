---
title: Accoutrement
type: class
superclass: Instance
---

# Accoutrement

An object that can attach to a player's character.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

An Accoutrement welds its child `Class.Part|part` called "Handle" to the
player's character. You can change the position and rotation of the Handle
part using the `Class.Accoutrement.AttachmentPos|AttachmentPos`,
`Class.Accoutrement.AttachmentRight|Right`,
`Class.Accoutrement.AttachmentForward|Forward`, and
`Class.Accoutrement.AttachmentUp|Up` properties.

Parts descending from an accoutrement are massless when attach to other parts
(e.g. with a Weld) as long as they are not the root part of the assembly that
`Class.BasePart:GetRootPart()|GetRootPart()` returns.
`Class.BasePart:GetMass()|GetMass()` returns 0 for parts in this case, and it
doesn't add to the total mass or rotational inertia of the Assembly.

This doesn't apply to a part descending from an accoutrement when an
accoutrement welds to another part that is massless or one if its parts
otherwise becomes root. This also doesn't apply for the root part, and it has
mass like a normal part.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Accoutrement.AttachmentForward` | `Datatype.Vector3` | [Hidden] [NotReplicated] |
| `Class.Accoutrement.AttachmentPoint` | `Datatype.CFrame` |  |
| `Class.Accoutrement.AttachmentPos` | `Datatype.Vector3` | [Hidden] [NotReplicated] |
| `Class.Accoutrement.AttachmentRight` | `Datatype.Vector3` | [Hidden] [NotReplicated] |
| `Class.Accoutrement.AttachmentUp` | `Datatype.Vector3` | [Hidden] [NotReplicated] |
