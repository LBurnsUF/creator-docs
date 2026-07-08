---
title: Pants
type: class
superclass: Clothing
---

# Pants

Displays a Pants texture from the Roblox website to display on a
`Class.Humanoid` rig.

**Inherits from:** `Class.Clothing` > `Class.CharacterAppearance` > `Class.Instance` > `Class.Object`

## Description

The `Pants` object displays a pants texture from Roblox on a `Class.Humanoid`
rig. Pants cover the torso and legs, and will be covered by a `Class.Shirt` on
the torso. To be visible, a `Pants` must be a sibling of a `Class.Humanoid`
and have its `Class.Pants.PantsTemplate|PantsTemplate` property set to an
appropriate texture such as `rbxassetid://86896501`. The pants texture may be
colorized using the `Class.Clothing.Color3` property.

Pants are automatically loaded on `Class.Player` characters if their avatar is
wearing one.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Pants.PantsTemplate` | `Datatype.ContentId` |  |
| `Class.Pants.PantsTemplateContent` | `Datatype.Content` |  |
