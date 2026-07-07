---
title: HumanoidDescription
type: class
superclass: Instance
---

# HumanoidDescription

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.HumanoidDescription.AccessoryBlob` | `string` | [NotReplicated] [NotScriptable] |
| `Class.HumanoidDescription.BackAccessory` | `string` | [NotReplicated] |
| `Class.HumanoidDescription.BodyTypeScale` | `float` |  |
| `Class.HumanoidDescription.ClimbAnimation` | `int64` |  |
| `Class.HumanoidDescription.DepthScale` | `float` |  |
| `Class.HumanoidDescription.Face` | `int64` |  |
| `Class.HumanoidDescription.FaceAccessory` | `string` | [NotReplicated] |
| `Class.HumanoidDescription.FallAnimation` | `int64` |  |
| `Class.HumanoidDescription.FrontAccessory` | `string` | [NotReplicated] |
| `Class.HumanoidDescription.GraphicTShirt` | `int64` |  |
| `Class.HumanoidDescription.HairAccessory` | `string` | [NotReplicated] |
| `Class.HumanoidDescription.HatAccessory` | `string` | [NotReplicated] |
| `Class.HumanoidDescription.Head` | `int64` | [NotReplicated] |
| `Class.HumanoidDescription.HeadColor` | `Datatype.Color3` | [NotReplicated] |
| `Class.HumanoidDescription.HeadScale` | `float` |  |
| `Class.HumanoidDescription.HeightScale` | `float` |  |
| `Class.HumanoidDescription.IdleAnimation` | `int64` |  |
| `Class.HumanoidDescription.JumpAnimation` | `int64` |  |
| `Class.HumanoidDescription.LeftArm` | `int64` | [NotReplicated] |
| `Class.HumanoidDescription.LeftArmColor` | `Datatype.Color3` | [NotReplicated] |
| `Class.HumanoidDescription.LeftLeg` | `int64` | [NotReplicated] |
| `Class.HumanoidDescription.LeftLegColor` | `Datatype.Color3` | [NotReplicated] |
| `Class.HumanoidDescription.MoodAnimation` | `int64` |  |
| `Class.HumanoidDescription.NeckAccessory` | `string` | [NotReplicated] |
| `Class.HumanoidDescription.NumberEmotesLoaded` | `int` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.HumanoidDescription.Pants` | `int64` |  |
| `Class.HumanoidDescription.ProportionScale` | `float` |  |
| `Class.HumanoidDescription.ResetIncludesBodyParts` | `bool` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.HumanoidDescription.RightArm` | `int64` | [NotReplicated] |
| `Class.HumanoidDescription.RightArmColor` | `Datatype.Color3` | [NotReplicated] |
| `Class.HumanoidDescription.RightLeg` | `int64` | [NotReplicated] |
| `Class.HumanoidDescription.RightLegColor` | `Datatype.Color3` | [NotReplicated] |
| `Class.HumanoidDescription.RunAnimation` | `int64` |  |
| `Class.HumanoidDescription.Shirt` | `int64` |  |
| `Class.HumanoidDescription.ShouldersAccessory` | `string` | [NotReplicated] |
| `Class.HumanoidDescription.StaticFacialAnimation` | `bool` |  |
| `Class.HumanoidDescription.SwimAnimation` | `int64` |  |
| `Class.HumanoidDescription.Torso` | `int64` | [NotReplicated] |
| `Class.HumanoidDescription.TorsoColor` | `Datatype.Color3` | [NotReplicated] |
| `Class.HumanoidDescription.UseAvatarSettings` | `bool` |  |
| `Class.HumanoidDescription.WaistAccessory` | `string` | [NotReplicated] |
| `Class.HumanoidDescription.WalkAnimation` | `int64` |  |
| `Class.HumanoidDescription.WidthScale` | `float` |  |

## Methods

### `Class.HumanoidDescription:AddEmote`

``AddEmote(name: `string`, assetId: `int64`)`` → `null`

### `Class.HumanoidDescription:GetAccessories`

``GetAccessories(includeRigidAccessories: `bool`)`` → `Array`

### `Class.HumanoidDescription:GetEmotes`

``GetEmotes()`` → `Dictionary`

### `Class.HumanoidDescription:GetEquippedEmotes`

``GetEquippedEmotes()`` → `Array`

### `Class.HumanoidDescription:RemoveEmote`

``RemoveEmote(name: `string`)`` → `null`

### `Class.HumanoidDescription:SetAccessories`

``SetAccessories(accessories: `Array`, includeRigidAccessories: `bool`)`` → `null`

### `Class.HumanoidDescription:SetEmotes`

``SetEmotes(emotes: `Dictionary`)`` → `null`

### `Class.HumanoidDescription:SetEquippedEmotes`

``SetEquippedEmotes(equippedEmotes: `Array`)`` → `null`

## Events

### `Class.HumanoidDescription.EmotesChanged`

Fires with: (newEmotes: `Dictionary`)

### `Class.HumanoidDescription.EquippedEmotesChanged`

Fires with: (newEquippedEmotes: `Array`)
