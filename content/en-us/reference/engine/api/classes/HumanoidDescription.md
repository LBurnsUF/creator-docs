---
title: HumanoidDescription
type: class
superclass: Instance
---

# HumanoidDescription

**Inherits**: Instance > Object

## Properties

- **AccessoryBlob**: `string` [NotReplicated] [NotScriptable]
- **BackAccessory**: `string` [NotReplicated]
- **BodyTypeScale**: `float`
- **ClimbAnimation**: `int64`
- **DepthScale**: `float`
- **Face**: `int64`
- **FaceAccessory**: `string` [NotReplicated]
- **FallAnimation**: `int64`
- **FrontAccessory**: `string` [NotReplicated]
- **GraphicTShirt**: `int64`
- **HairAccessory**: `string` [NotReplicated]
- **HatAccessory**: `string` [NotReplicated]
- **Head**: `int64` [NotReplicated]
- **HeadColor**: `Color3` [NotReplicated]
- **HeadScale**: `float`
- **HeightScale**: `float`
- **IdleAnimation**: `int64`
- **JumpAnimation**: `int64`
- **LeftArm**: `int64` [NotReplicated]
- **LeftArmColor**: `Color3` [NotReplicated]
- **LeftLeg**: `int64` [NotReplicated]
- **LeftLegColor**: `Color3` [NotReplicated]
- **MoodAnimation**: `int64`
- **NeckAccessory**: `string` [NotReplicated]
- **NumberEmotesLoaded**: `int` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Pants**: `int64`
- **ProportionScale**: `float`
- **ResetIncludesBodyParts**: `bool` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **RightArm**: `int64` [NotReplicated]
- **RightArmColor**: `Color3` [NotReplicated]
- **RightLeg**: `int64` [NotReplicated]
- **RightLegColor**: `Color3` [NotReplicated]
- **RunAnimation**: `int64`
- **Shirt**: `int64`
- **ShouldersAccessory**: `string` [NotReplicated]
- **StaticFacialAnimation**: `bool`
- **SwimAnimation**: `int64`
- **Torso**: `int64` [NotReplicated]
- **TorsoColor**: `Color3` [NotReplicated]
- **UseAvatarSettings**: `bool`
- **WaistAccessory**: `string` [NotReplicated]
- **WalkAnimation**: `int64`
- **WidthScale**: `float`

## Methods

- **AddEmote**(`name: string`, `assetId: int64`) -> `null`
- **GetAccessories**(`includeRigidAccessories: bool`) -> `Array`
- **GetEmotes**() -> `Dictionary`
- **GetEquippedEmotes**() -> `Array`
- **RemoveEmote**(`name: string`) -> `null`
- **SetAccessories**(`accessories: Array`, `includeRigidAccessories: bool`) -> `null`
- **SetEmotes**(`emotes: Dictionary`) -> `null`
- **SetEquippedEmotes**(`equippedEmotes: Array`) -> `null`

## Events

- **EmotesChanged**(`newEmotes: Dictionary`)
- **EquippedEmotesChanged**(`newEquippedEmotes: Array`)
