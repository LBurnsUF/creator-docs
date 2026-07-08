---
title: StarterPlayer
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# StarterPlayer

A service which allows the defaults of properties in the `Class.Player` object
to be set.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

A service which allows the defaults of properties in the `Class.Player` object
to be set. When a player enters the server, each property of the player object
is set to the current value of the corresponding property in
`Class.StarterPlayer`.

Additionally, you may add four objects to this service:

- A `Class.StarterPlayerScripts` instance with scripts that run once for each
  player.
- A `Class.StarterCharacterScripts` instance with scripts to add to each
  player's character every time they spawn.
- A `Class.Humanoid` instance named `StarterHumanoid` which will be used as
  the default humanoid for each player's character.
- A `Class.Model` instance named `StarterCharacter` which will be used as the
  character model for all players.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.StarterPlayer.AllowCustomAnimations` | `bool` | [Hidden] {write: RobloxScriptSecurity} |
| `Class.StarterPlayer.AutoJumpEnabled` | `bool` |  |
| `Class.StarterPlayer.AvatarJointUpgrade` | `Enum.RolloutState` | [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StarterPlayer.CameraMaxZoomDistance` | `float` |  |
| `Class.StarterPlayer.CameraMinZoomDistance` | `float` |  |
| `Class.StarterPlayer.CameraMode` | `Enum.CameraMode` |  |
| `Class.StarterPlayer.CharacterBreakJointsOnDeath` | `bool` |  |
| `Class.StarterPlayer.CharacterJumpHeight` | `float` |  |
| `Class.StarterPlayer.CharacterJumpPower` | `float` |  |
| `Class.StarterPlayer.CharacterMaxSlopeAngle` | `float` |  |
| `Class.StarterPlayer.CharacterUseJumpPower` | `bool` |  |
| `Class.StarterPlayer.CharacterWalkSpeed` | `float` |  |
| `Class.StarterPlayer.ClassicDeath` | `bool` |  |
| `Class.StarterPlayer.CreateDefaultPlayerModule` | `bool` | [NotScriptable] |
| `Class.StarterPlayer.DevCameraOcclusionMode` | `Enum.DevCameraOcclusionMode` |  |
| `Class.StarterPlayer.DevComputerCameraMovementMode` | `Enum.DevComputerCameraMovementMode` |  |
| `Class.StarterPlayer.DevComputerMovementMode` | `Enum.DevComputerMovementMode` |  |
| `Class.StarterPlayer.DevTouchCameraMovementMode` | `Enum.DevTouchCameraMovementMode` |  |
| `Class.StarterPlayer.DevTouchMovementMode` | `Enum.DevTouchMovementMode` |  |
| `Class.StarterPlayer.EnableDynamicHeads` | `Enum.LoadDynamicHeads` | [NotScriptable] |
| `Class.StarterPlayer.EnableMouseLockOption` | `bool` |  |
| `Class.StarterPlayer.GameSettingsAssetIDFace` | `int64` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StarterPlayer.GameSettingsAssetIDHead` | `int64` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StarterPlayer.GameSettingsAssetIDLeftArm` | `int64` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StarterPlayer.GameSettingsAssetIDLeftLeg` | `int64` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StarterPlayer.GameSettingsAssetIDPants` | `int64` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StarterPlayer.GameSettingsAssetIDRightArm` | `int64` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StarterPlayer.GameSettingsAssetIDRightLeg` | `int64` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StarterPlayer.GameSettingsAssetIDShirt` | `int64` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StarterPlayer.GameSettingsAssetIDTeeShirt` | `int64` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StarterPlayer.GameSettingsAssetIDTorso` | `int64` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StarterPlayer.GameSettingsAvatar` | `Enum.GameAvatarType` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.StarterPlayer.GameSettingsR15Collision` | `Enum.R15CollisionType` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StarterPlayer.GameSettingsScaleRangeBodyType` | `Datatype.NumberRange` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StarterPlayer.GameSettingsScaleRangeHead` | `Datatype.NumberRange` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StarterPlayer.GameSettingsScaleRangeHeight` | `Datatype.NumberRange` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StarterPlayer.GameSettingsScaleRangeProportion` | `Datatype.NumberRange` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StarterPlayer.GameSettingsScaleRangeWidth` | `Datatype.NumberRange` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StarterPlayer.HealthDisplayDistance` | `float` |  |
| `Class.StarterPlayer.LoadCharacterAppearance` | `bool` |  |
| `Class.StarterPlayer.LoadCharacterLayeredClothing ` | `Enum.LoadCharacterLayeredClothing` | [NotReplicated] [NotScriptable] |
| `Class.StarterPlayer.LuaCharacterController` | `Enum.CharacterControlMode` |  |
| `Class.StarterPlayer.NameDisplayDistance` | `float` |  |
| `Class.StarterPlayer.PlayerModuleStatus` | `int` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.StarterPlayer.UserEmotesEnabled` | `bool` |  |

## Methods

### `Class.StarterPlayer:ClearDefaults`

``ClearDefaults()`` -> `null`
   {security: RobloxScriptSecurity}
