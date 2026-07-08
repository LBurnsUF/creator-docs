---
title: Shirt
type: class
superclass: Clothing
---

# Shirt

Displays a shirt texture on a `Class.Humanoid` rig.

**Inherits from:** `Class.Clothing` > `Class.CharacterAppearance` > `Class.Instance` > `Class.Object`

## Description

The `Shirt` object displays a shirt texture from Roblox on a `Class.Humanoid`
rig. Shirts cover the torso and arms, and will take priority over a
`Class.Pants` on the torso. To be visible, a `Shirt` must be a sibling of a
`Class.Humanoid` and have its `Class.Shirt.ShirtTemplate|ShirtTemplate`
property set to an appropriate texture such as `rbxassetid://86896487`. The
shirt texture may be colorized using the `Class.Clothing.Color3` property.

Shirts are automatically loaded on `Class.Player` characters if their avatar
is wearing one.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Shirt.ShirtTemplate` | `Datatype.ContentId` |  |
| `Class.Shirt.ShirtTemplateContent` | `Datatype.Content` |  |
