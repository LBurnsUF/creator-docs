---
title: Player
type: class
superclass: Instance
---

# Player

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.Player.AccountAge` | `int` | [ReadOnly] [NotReplicated] |
| `Class.Player.AgeChecked` | `Enum.AgeCheckStatus` |  {write: RobloxSecurity} |
| `Class.Player.AppearanceDidLoad` | `bool` | [Hidden] [ReadOnly] [NotReplicated] [Deprecated] {security: RobloxScriptSecurity} |
| `Class.Player.AutoJumpEnabled` | `bool` |  |
| `Class.Player.CameraMaxZoomDistance` | `float` |  |
| `Class.Player.CameraMinZoomDistance` | `float` |  |
| `Class.Player.CameraMode` | `Enum.CameraMode` |  |
| `Class.Player.CanLoadCharacterAppearance` | `bool` |  |
| `Class.Player.Character` | `Class.Model` |  |
| `Class.Player.CharacterAppearance` | `string` | [NotBrowsable] [Deprecated] |
| `Class.Player.CharacterAppearanceId` | `int64` |  |
| `Class.Player.ChatAvailabilityStatus` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Player.ChatMode` | `Enum.ChatMode` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Player.DataComplexity` | `int` | [Hidden] [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.Player.DataComplexityLimit` | `int` | [Hidden] [NotReplicated] [Deprecated] {security: LocalUserSecurity} |
| `Class.Player.DataReady` | `bool` | [Hidden] [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.Player.DevCameraOcclusionMode` | `Enum.DevCameraOcclusionMode` |  |
| `Class.Player.DevComputerCameraMode` | `Enum.DevComputerCameraMovementMode` |  |
| `Class.Player.DevComputerMovementMode` | `Enum.DevComputerMovementMode` |  |
| `Class.Player.DevEnableMouseLock` | `bool` |  |
| `Class.Player.DevTouchCameraMode` | `Enum.DevTouchCameraMovementMode` |  |
| `Class.Player.DevTouchMovementMode` | `Enum.DevTouchMovementMode` |  |
| `Class.Player.DisplayName` | `string` |  |
| `Class.Player.FollowUserId` | `int64` | [ReadOnly] [NotReplicated] |
| `Class.Player.GameplayPaused` | `bool` | [Hidden] {write: NotAccessibleSecurity} |
| `Class.Player.Guest` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Player.HasRobloxSubscription` | `bool` |  {write: RobloxSecurity} |
| `Class.Player.HasVerifiedBadge` | `bool` |  |
| `Class.Player.HealthDisplayDistance` | `float` |  |
| `Class.Player.InputLatency` | `int` |  {security: RobloxSecurity} |
| `Class.Player.LocaleId` | `string` | [Hidden] [ReadOnly] [NotReplicated] |
| `Class.Player.MaximumSimulationRadius` | `float` | [Hidden] [NotReplicated] {security: LocalUserSecurity} |
| `Class.Player.MembershipType` | `Enum.MembershipType` | [ReadOnly] [NotReplicated] |
| `Class.Player.NameDisplayDistance` | `float` |  |
| `Class.Player.Neutral` | `bool` |  |
| `Class.Player.OsPlatform` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Player.PartyId` | `string` | [Hidden] [NotReplicated] {write: RobloxSecurity} |
| `Class.Player.PlatformName` | `string` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.Player.ReplicationFocus` | `Class.Instance` |  |
| `Class.Player.RespawnLocation` | `Class.SpawnLocation` |  |
| `Class.Player.SimulationRadius` | `float` | [Hidden] {security: LocalUserSecurity} |
| `Class.Player.StepIdOffset` | `int` |  {security: RobloxSecurity} |
| `Class.Player.Team` | `Class.Team` | [NotReplicated] |
| `Class.Player.TeamColor` | `Datatype.BrickColor` |  |
| `Class.Player.Teleported` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Player.TeleportedIn` | `bool` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.Player.ThirdPartyTextChatRestrictionStatus` | `Enum.ChatRestrictionStatus` | [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Player.UnfilteredChat` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Player.User` | `Datatype.User` |  {write: RobloxSecurity} |
| `Class.Player.UserId` | `int64` |  |
| `Class.Player.VRDevice` | `string` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.Player.VREnabled` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Player.userId` | `int64` | [Deprecated] |

## Methods

### `Class.Player:AddReplicationFocus`

``AddReplicationFocus(part: `Class.BasePart`)`` → `null`

### `Class.Player:AddReplicationFocusPosition`

``AddReplicationFocusPosition(center: `Datatype.Vector3`, radius: `int`)`` → `null`
   {security: RobloxSecurity}

### `Class.Player:AddToBlockList`

``AddToBlockList(userIds: `Array`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Player:ClearCachedAvatarAppearance`

``ClearCachedAvatarAppearance()`` → `null`

### `Class.Player:ClearCharacterAppearance`

``ClearCharacterAppearance()`` → `null`

### `Class.Player:DistanceFromCharacter`

``DistanceFromCharacter(point: `Datatype.Vector3`)`` → `float`

### `Class.Player:GetBlockListInitialized`

``GetBlockListInitialized()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.Player:GetCameraState`

``GetCameraState()`` → `Dictionary`
  [CustomLuaState]

### `Class.Player:GetCanManageAsync`

``GetCanManageAsync()`` → `bool`
  [Yields] {security: RobloxScriptSecurity}

### `Class.Player:GetData`

``GetData()`` → `Class.PlayerData`

### `Class.Player:GetFriendStatus`

``GetFriendStatus(player: `Class.Player`)`` → `Enum.FriendStatus`
   {security: RobloxScriptSecurity}

### `Class.Player:GetFriendsOnline`

``GetFriendsOnline(maxFriends: `int`)`` → `Array`
  [Yields] [Deprecated]

### `Class.Player:GetFriendsOnlineAsync`

``GetFriendsOnlineAsync(maxFriends: `int`)`` → `Array`
  [Yields]

### `Class.Player:GetFriendsWhoPlayedAsync`

``GetFriendsWhoPlayedAsync()`` → `Array`
  [Yields]

### `Class.Player:GetGameSessionID`

``GetGameSessionID()`` → `string`
   {security: RobloxSecurity}

### `Class.Player:GetJoinData`

``GetJoinData()`` → `Dictionary`
  [CustomLuaState]

### `Class.Player:GetMouse`

``GetMouse()`` → `Class.Mouse`

### `Class.Player:GetNetworkPing`

``GetNetworkPing()`` → `float`

### `Class.Player:GetRankInGroup`

``GetRankInGroup(groupId: `int64`)`` → `int`
  [Yields] [Deprecated]

### `Class.Player:GetRankInGroupAsync`

``GetRankInGroupAsync(groupId: `int64`)`` → `int`
  [Yields] [Deprecated]

### `Class.Player:GetRoleInGroup`

``GetRoleInGroup(groupId: `int64`)`` → `string`
  [Yields] [Deprecated]

### `Class.Player:GetRoleInGroupAsync`

``GetRoleInGroupAsync(groupId: `int64`)`` → `string`
  [Yields] [Deprecated]

### `Class.Player:GetSeatRequested`

``GetSeatRequested()`` → `Class.Instance`
   {security: RobloxScriptSecurity}

### `Class.Player:GetToolRequested`

``GetToolRequested()`` → `Class.Instance`
   {security: RobloxScriptSecurity}

### `Class.Player:GetUnder13`

``GetUnder13()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.Player:HasAppearanceLoaded`

``HasAppearanceLoaded()`` → `bool`

### `Class.Player:HasBlockedPlayer`

``HasBlockedPlayer(fromPlayer: `int64`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.Player:IsBestFriendsWith`

``IsBestFriendsWith(userId: `Datatype.User`)`` → `bool`
  [Yields] [Deprecated]

### `Class.Player:IsFriendsWith`

``IsFriendsWith(userId: `Datatype.User`)`` → `bool`
  [Yields] [Deprecated]

### `Class.Player:IsFriendsWithAsync`

``IsFriendsWithAsync(userId: `Datatype.User`)`` → `bool`
  [Yields]

### `Class.Player:IsInGroup`

``IsInGroup(groupId: `int64`)`` → `bool`
  [Yields] [Deprecated]

### `Class.Player:IsInGroupAsync`

``IsInGroupAsync(groupId: `int64`)`` → `bool`
  [Yields]

### `Class.Player:IsVerified`

``IsVerified()`` → `bool`

### `Class.Player:Kick`

``Kick(message: `string`)`` → `null`

### `Class.Player:LoadBoolean`

``LoadBoolean(key: `string`)`` → `bool`
  [Deprecated]

### `Class.Player:LoadCharacter`

``LoadCharacter()`` → `null`
  [Yields] [Deprecated]

### `Class.Player:LoadCharacterAppearance`

``LoadCharacterAppearance(assetInstance: `Class.Instance`)`` → `null`
  [Deprecated]

### `Class.Player:LoadCharacterAsync`

``LoadCharacterAsync()`` → `null`
  [Yields]

### `Class.Player:LoadCharacterBlocking`

``LoadCharacterBlocking()`` → `null`
  [Yields] {security: LocalUserSecurity}

### `Class.Player:LoadCharacterWithAvatarRules`

``LoadCharacterWithAvatarRules(avatarRules: `Class.AvatarRules`)`` → `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.Player:LoadCharacterWithHumanoidDescription`

``LoadCharacterWithHumanoidDescription(humanoidDescription: `Class.HumanoidDescription`, assetTypeVerification: `Enum.AssetTypeVerification`)`` → `null`
  [Yields] [Deprecated]

### `Class.Player:LoadCharacterWithHumanoidDescriptionAsync`

``LoadCharacterWithHumanoidDescriptionAsync(humanoidDescription: `Class.HumanoidDescription`, assetTypeVerification: `Enum.AssetTypeVerification`)`` → `null`
  [Yields]

### `Class.Player:LoadData`

``LoadData()`` → `null`
  [Deprecated] {security: LocalUserSecurity}

### `Class.Player:LoadInstance`

``LoadInstance(key: `string`)`` → `Class.Instance`
  [Deprecated]

### `Class.Player:LoadNumber`

``LoadNumber(key: `string`)`` → `double`
  [Deprecated]

### `Class.Player:LoadString`

``LoadString(key: `string`)`` → `string`
  [Deprecated]

### `Class.Player:Move`

``Move(walkDirection: `Datatype.Vector3`, relativeToCamera: `bool`)`` → `null`

### `Class.Player:NotifyAgeCheckPassed`

``NotifyAgeCheckPassed()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Player:OverrideStreamingRadii`

``OverrideStreamingRadii(minRadius: `int`, targetRadius: `int`)`` → `null`
   {security: RobloxSecurity}

### `Class.Player:PinStreamingForInstance`

``PinStreamingForInstance(instance: `Class.Instance`, depth: `int`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Player:PinStreamingForInstanceByUniqueId`

``PinStreamingForInstanceByUniqueId(uniqueIdString: `string`, depth: `int`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Player:PromptAgeCheck`

``PromptAgeCheck()`` → `null`

### `Class.Player:PromptSecurityChallengeAsync`

``PromptSecurityChallengeAsync()`` → `bool`
  [Yields] {security: RobloxSecurity}

### `Class.Player:RemoveCharacter`

``RemoveCharacter()`` → `null`
   {security: LocalUserSecurity}

### `Class.Player:RemoveReplicationFocus`

``RemoveReplicationFocus(part: `Class.BasePart`)`` → `null`

### `Class.Player:RemoveReplicationFocusPosition`

``RemoveReplicationFocusPosition(center: `Datatype.Vector3`, radius: `int`)`` → `null`
   {security: RobloxSecurity}

### `Class.Player:RequestFriendship`

``RequestFriendship(player: `Class.Player`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Player:RequestSeat`

``RequestSeat(instance: `Class.Instance`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Player:RequestStreamAroundAsync`

``RequestStreamAroundAsync(position: `Datatype.Vector3`, timeOut: `double`)`` → `null`
  [Yields]

### `Class.Player:RequestTool`

``RequestTool(instance: `Class.Instance`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Player:RevokeFriendship`

``RevokeFriendship(player: `Class.Player`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Player:SaveBoolean`

``SaveBoolean(key: `string`, value: `bool`)`` → `null`
  [Deprecated]

### `Class.Player:SaveData`

``SaveData()`` → `null`
  [Deprecated] {security: LocalUserSecurity}

### `Class.Player:SaveInstance`

``SaveInstance(key: `string`, value: `Class.Instance`)`` → `null`
  [Deprecated]

### `Class.Player:SaveNumber`

``SaveNumber(key: `string`, value: `double`)`` → `null`
  [Deprecated]

### `Class.Player:SaveString`

``SaveString(key: `string`, value: `string`)`` → `null`
  [Deprecated]

### `Class.Player:SetAccountAge`

``SetAccountAge(accountAge: `int`)`` → `null`
   {security: PluginSecurity}

### `Class.Player:SetBlockListInitialized`

``SetBlockListInitialized()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Player:SetCharacterAppearanceJson`

``SetCharacterAppearanceJson(jsonBlob: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Player:SetChatTranslationSettingsLocaleId`

``SetChatTranslationSettingsLocaleId(locale: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Player:SetExperienceSettingsLocaleId`

``SetExperienceSettingsLocaleId(locale: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Player:SetHasRobloxSubscription`

``SetHasRobloxSubscription(hasRobloxSubscription: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Player:SetMembershipType`

``SetMembershipType(membershipType: `Enum.MembershipType`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Player:SetModerationAccessKey`

``SetModerationAccessKey(moderationAccessKey: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Player:SetSuperSafeChat`

``SetSuperSafeChat(value: `bool`)`` → `null`
   {security: PluginSecurity}

### `Class.Player:SetUnder13`

``SetUnder13(value: `bool`)`` → `null`
  [Deprecated] {security: RobloxSecurity}

### `Class.Player:UnpinStreamingForInstance`

``UnpinStreamingForInstance(instance: `Class.Instance`, depth: `int`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Player:UpdatePlayerBlocked`

``UpdatePlayerBlocked(userId: `int64`, blocked: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Player:WaitForDataReady`

``WaitForDataReady()`` → `bool`
  [Yields] [Deprecated]

### `Class.Player:isFriendsWith`

``isFriendsWith(userId: `Datatype.User`)`` → `bool`
  [Yields] [Deprecated]

### `Class.Player:loadBoolean`

``loadBoolean(key: `string`)`` → `bool`
  [Deprecated]

### `Class.Player:loadInstance`

``loadInstance(key: `string`)`` → `Class.Instance`
  [Deprecated]

### `Class.Player:loadNumber`

``loadNumber(key: `string`)`` → `double`
  [Deprecated]

### `Class.Player:loadString`

``loadString(key: `string`)`` → `string`
  [Deprecated]

### `Class.Player:saveBoolean`

``saveBoolean(key: `string`, value: `bool`)`` → `null`
  [Deprecated]

### `Class.Player:saveInstance`

``saveInstance(key: `string`, value: `Class.Instance`)`` → `null`
  [Deprecated]

### `Class.Player:saveNumber`

``saveNumber(key: `string`, value: `double`)`` → `null`
  [Deprecated]

### `Class.Player:saveString`

``saveString(key: `string`, value: `string`)`` → `null`
  [Deprecated]

### `Class.Player:waitForDataReady`

``waitForDataReady()`` → `bool`
  [Yields] [Deprecated]

## Events

### `Class.Player.BlockListChanged`

Fires with: ()

### `Class.Player.CharacterAdded`

Fires with: (character: `Class.Model`)

### `Class.Player.CharacterAppearanceLoaded`

Fires with: (character: `Class.Model`)

### `Class.Player.CharacterRemoving`

Fires with: (character: `Class.Model`)

### `Class.Player.Chatted`

Fires with: (message: `string`, recipient: `Class.Player`)

### `Class.Player.CloudEditSelectionChanged`

Fires with: (newSelection: `Array`)

### `Class.Player.FriendStatusChanged`

Fires with: (player: `Class.Player`, friendStatus: `Enum.FriendStatus`)

### `Class.Player.Idled`

Fires with: (time: `double`)

### `Class.Player.InstancePinned`

Fires with: (uniqueIdString: `string`, depth: `int`)

### `Class.Player.InstanceUnpinned`

Fires with: (uniqueIdString: `string`, depth: `int`)

### `Class.Player.OnTeleport`

Fires with: (teleportState: `Enum.TeleportState`, placeId: `int64`, spawnName: `string`)

### `Class.Player.SimulationRadiusChanged`

Fires with: (radius: `float`)

### `Class.Player.StreamingPinComplete`

Fires with: (instance: `Class.Instance`)
