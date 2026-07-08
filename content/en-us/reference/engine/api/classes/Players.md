---
title: Players
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# Players

A service that contains presently connected `Class.Player` objects.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

The `Class.Players` service contains `Class.Player` objects for presently
connected clients to a Roblox server. It also contains information about a
place's configuration. It can fetch information about players not connected to
the server, such as character appearances, friends, and avatar thumbnail.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Players.BanningEnabled` | `bool` | [NotScriptable] |
| `Class.Players.BubbleChat` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.Players.CharacterAutoLoads` | `bool` | [NotReplicated] |
| `Class.Players.ClassicChat` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.Players.LocalPlayer` | `Class.Player` | [ReadOnly] [NotReplicated] |
| `Class.Players.MaxPlayers` | `int` | [ReadOnly] [NotReplicated] |
| `Class.Players.MaxPlayersInternal` | `int` | [Hidden] {security: LocalUserSecurity} |
| `Class.Players.NumPlayers` | `int` | [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.Players.PreferredPlayers` | `int` | [ReadOnly] [NotReplicated] |
| `Class.Players.PreferredPlayersInternal` | `int` | [Hidden] {security: LocalUserSecurity} |
| `Class.Players.RespawnTime` | `float` |  |
| `Class.Players.UseStrafingAnimations` | `bool` | [NotScriptable] |
| `Class.Players.localPlayer` | `Class.Player` | [Hidden] [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.Players.numPlayers` | `int` | [Hidden] [ReadOnly] [NotReplicated] [Deprecated] |

## Methods

### `Class.Players:BanAsync`

``BanAsync(config: `Dictionary`)`` -> `null`
  [Yields]

### `Class.Players:Chat`

``Chat(message: `string`)`` -> `null`
   {security: PluginSecurity}

### `Class.Players:CreateHumanoidModelFromDescription`

``CreateHumanoidModelFromDescription(description: `Class.HumanoidDescription`, rigType: `Enum.HumanoidRigType`, assetTypeVerification: `Enum.AssetTypeVerification`)`` -> `Class.Model`
  [Yields] [Deprecated]

### `Class.Players:CreateHumanoidModelFromDescriptionAsync`

``CreateHumanoidModelFromDescriptionAsync(description: `Class.HumanoidDescription`, rigType: `Enum.HumanoidRigType`, assetTypeVerification: `Enum.AssetTypeVerification`)`` -> `Class.Model`
  [Yields]

### `Class.Players:CreateHumanoidModelFromUserId`

``CreateHumanoidModelFromUserId(userId: `Datatype.User`)`` -> `Class.Model`
  [Yields] [Deprecated]

### `Class.Players:CreateHumanoidModelFromUserIdAsync`

``CreateHumanoidModelFromUserIdAsync(userId: `Datatype.User`)`` -> `Class.Model`
  [Yields]

### `Class.Players:CreateLocalPlayer`

``CreateLocalPlayer()`` -> `Class.Player`
   {security: LocalUserSecurity}

### `Class.Players:CreateThumbnailPlayer`

``CreateThumbnailPlayer()`` -> `Class.Player`
   {security: RobloxScriptSecurity}

### `Class.Players:GetBanHistoryAsync`

``GetBanHistoryAsync(userId: `Datatype.User`)`` -> `Class.BanHistoryPages`
  [Yields]

### `Class.Players:GetCharacterAppearanceAsync`

``GetCharacterAppearanceAsync(userId: `Datatype.User`)`` -> `Class.Model`
  [Yields] [Deprecated]

### `Class.Players:GetCharacterAppearanceInfoAsync`

``GetCharacterAppearanceInfoAsync(userId: `Datatype.User`)`` -> `Dictionary`
  [Yields]

### `Class.Players:GetFriendsAsync`

``GetFriendsAsync(userId: `Datatype.User`)`` -> `Class.FriendPages`
  [Yields]

### `Class.Players:GetHumanoidDescriptionFromOutfitId`

``GetHumanoidDescriptionFromOutfitId(outfitId: `int64`)`` -> `Class.HumanoidDescription`
  [Yields] [Deprecated]

### `Class.Players:GetHumanoidDescriptionFromOutfitIdAsync`

``GetHumanoidDescriptionFromOutfitIdAsync(outfitId: `int64`)`` -> `Class.HumanoidDescription`
  [Yields]

### `Class.Players:GetHumanoidDescriptionFromUserId`

``GetHumanoidDescriptionFromUserId(userId: `Datatype.User`)`` -> `Class.HumanoidDescription`
  [Yields] [Deprecated]

### `Class.Players:GetHumanoidDescriptionFromUserIdAsync`

``GetHumanoidDescriptionFromUserIdAsync(userId: `Datatype.User`)`` -> `Class.HumanoidDescription`
  [Yields]

### `Class.Players:GetNameFromUserIdAsync`

``GetNameFromUserIdAsync(userId: `Datatype.User`)`` -> `string`
  [Yields]

### `Class.Players:GetPlayerByUserId`

``GetPlayerByUserId(userId: `Datatype.User`)`` -> `Class.Player`

### `Class.Players:GetPlayerFromCharacter`

``GetPlayerFromCharacter(character: `Class.Model`)`` -> `Class.Player`

### `Class.Players:GetPlayers`

``GetPlayers()`` -> `Datatype.Instances`

### `Class.Players:GetProfileConfigurationFromUserIdAsync`

``GetProfileConfigurationFromUserIdAsync(userId: `Datatype.User`)`` -> `Dictionary`
  [Yields]

### `Class.Players:GetUserIdFromNameAsync`

``GetUserIdFromNameAsync(userName: `string`)`` -> `int64`
  [Yields]

### `Class.Players:GetUserThumbnailAsync`

``GetUserThumbnailAsync(userId: `Datatype.User`, thumbnailType: `Enum.ThumbnailType`, thumbnailSize: `Enum.ThumbnailSize`)`` -> `Tuple`
  [Yields]

### `Class.Players:ReportAbuse`

``ReportAbuse(player: `Class.Player`, reason: `string`, optionalMessage: `string`)`` -> `null`
   {security: LocalUserSecurity}

### `Class.Players:ReportAbuseV3`

``ReportAbuseV3(player: `Class.Player`, jsonTags: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.Players:ReportAvatarAbuse`

``ReportAvatarAbuse(targetUserId: `int64`, tags: `Dictionary`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.Players:ReportChatAbuse`

``ReportChatAbuse(eligibleChatLines: `Array`, targetChatLines: `Array`, tags: `Dictionary`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.Players:ResetLocalPlayer`

``ResetLocalPlayer()`` -> `null`
   {security: LocalUserSecurity}

### `Class.Players:SetChatStyle`

``SetChatStyle(style: `Enum.ChatStyle`)`` -> `null`
   {security: PluginSecurity}

### `Class.Players:SetLocalPlayerInfo`

``SetLocalPlayerInfo(userId: `int64`, userName: `string`, displayName: `string`, membershipType: `Enum.MembershipType`, isUnder13: `bool`, hasRobloxSubscription: `bool`, ageCheckedStatus: `Enum.AgeCheckStatus`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.Players:TeamChat`

``TeamChat(message: `string`)`` -> `null`
   {security: PluginSecurity}

### `Class.Players:UnbanAsync`

``UnbanAsync(config: `Dictionary`)`` -> `null`
  [Yields]

### `Class.Players:WhisperChat`

``WhisperChat(message: `string`, player: `Class.Instance`)`` -> `null`
   {security: LocalUserSecurity}

### `Class.Players:getPlayers`

``getPlayers()`` -> `Datatype.Instances`
  [Deprecated]

### `Class.Players:playerFromCharacter`

``playerFromCharacter(character: `Class.Model`)`` -> `Class.Player`
  [Deprecated]

### `Class.Players:players`

``players()`` -> `Datatype.Instances`
  [Deprecated]

## Events

### `Class.Players.FriendRequestEvent`

Fires with: (player: `Class.Player`, player: `Class.Player`, friendRequestEvent: `Enum.FriendRequestEvent`)

### `Class.Players.PlayerAdded`

Fires with: (player: `Class.Player`)

### `Class.Players.PlayerChatted`

Fires with: (chatType: `Enum.PlayerChatType`, player: `Class.Player`, message: `string`, targetPlayer: `Class.Player`)

### `Class.Players.PlayerConnecting`

Fires with: (player: `Class.Player`)

### `Class.Players.PlayerDisconnecting`

Fires with: (player: `Class.Player`)

### `Class.Players.PlayerMembershipChanged`

Fires with: (player: `Class.Player`)

### `Class.Players.PlayerRejoining`

Fires with: (player: `Class.Player`)

### `Class.Players.PlayerRemoving`

Fires with: (player: `Class.Player`, reason: `Enum.PlayerExitReason`)

### `Class.Players.PromptAgeCheckRequested`

Fires with: (player: `Class.Player`)

### `Class.Players.UserSubscriptionStatusChanged`

Fires with: (user: `Class.Player`, subscriptionId: `string`)
