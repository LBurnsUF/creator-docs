---
title: Players
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# Players

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **BanningEnabled**: `bool` [NotScriptable]
- **BubbleChat**: `bool` [ReadOnly] [NotReplicated]
- **CharacterAutoLoads**: `bool` [NotReplicated]
- **ClassicChat**: `bool` [ReadOnly] [NotReplicated]
- **LocalPlayer**: `Player` [ReadOnly] [NotReplicated]
- **MaxPlayers**: `int` [ReadOnly] [NotReplicated]
- **MaxPlayersInternal**: `int` [Hidden] (Security: Read=LocalUserSecurity, Write=LocalUserSecurity)
- **NumPlayers**: `int` [ReadOnly] [NotReplicated] [Deprecated]
- **PreferredPlayers**: `int` [ReadOnly] [NotReplicated]
- **PreferredPlayersInternal**: `int` [Hidden] (Security: Read=LocalUserSecurity, Write=LocalUserSecurity)
- **RespawnTime**: `float`
- **UseStrafingAnimations**: `bool` [NotScriptable]
- **localPlayer**: `Player` [Hidden] [ReadOnly] [NotReplicated] [Deprecated]
- **numPlayers**: `int` [Hidden] [ReadOnly] [NotReplicated] [Deprecated]

## Methods

- **BanAsync**(`config: Dictionary`) -> `null` [Yields]
- **Chat**(`message: string`) -> `null`
- **CreateHumanoidModelFromDescription**(`description: HumanoidDescription`, `rigType: HumanoidRigType`, `assetTypeVerification: AssetTypeVerification = Default`) -> `Model` [Yields] [Deprecated]
- **CreateHumanoidModelFromDescriptionAsync**(`description: HumanoidDescription`, `rigType: HumanoidRigType`, `assetTypeVerification: AssetTypeVerification = Default`) -> `Model` [Yields]
- **CreateHumanoidModelFromUserId**(`userId: User`) -> `Model` [Yields] [Deprecated]
- **CreateHumanoidModelFromUserIdAsync**(`userId: User`) -> `Model` [Yields]
- **CreateLocalPlayer**() -> `Player`
- **CreateThumbnailPlayer**() -> `Player`
- **GetBanHistoryAsync**(`userId: User`) -> `BanHistoryPages` [Yields]
- **GetCharacterAppearanceAsync**(`userId: User`) -> `Model` [Yields] [Deprecated]
- **GetCharacterAppearanceInfoAsync**(`userId: User`) -> `Dictionary` [Yields]
- **GetFriendsAsync**(`userId: User`) -> `FriendPages` [Yields]
- **GetHumanoidDescriptionFromOutfitId**(`outfitId: int64`) -> `HumanoidDescription` [Yields] [Deprecated]
- **GetHumanoidDescriptionFromOutfitIdAsync**(`outfitId: int64`) -> `HumanoidDescription` [Yields]
- **GetHumanoidDescriptionFromUserId**(`userId: User`) -> `HumanoidDescription` [Yields] [Deprecated]
- **GetHumanoidDescriptionFromUserIdAsync**(`userId: User`) -> `HumanoidDescription` [Yields]
- **GetNameFromUserIdAsync**(`userId: User`) -> `string` [Yields]
- **GetPlayerByUserId**(`userId: User`) -> `Player`
- **GetPlayerFromCharacter**(`character: Model`) -> `Player`
- **GetPlayers**() -> `Instances`
- **GetProfileConfigurationFromUserIdAsync**(`userId: User`) -> `Dictionary` [Yields]
- **GetUserIdFromNameAsync**(`userName: string`) -> `int64` [Yields]
- **GetUserThumbnailAsync**(`userId: User`, `thumbnailType: ThumbnailType`, `thumbnailSize: ThumbnailSize`) -> `Tuple` [Yields]
- **ReportAbuse**(`player: Player`, `reason: string`, `optionalMessage: string`) -> `null`
- **ReportAbuseV3**(`player: Player`, `jsonTags: string`) -> `null`
- **ReportAvatarAbuse**(`targetUserId: int64`, `tags: Dictionary`) -> `null`
- **ReportChatAbuse**(`eligibleChatLines: Array`, `targetChatLines: Array`, `tags: Dictionary`) -> `null`
- **ResetLocalPlayer**() -> `null`
- **SetChatStyle**(`style: ChatStyle = Classic`) -> `null`
- **SetLocalPlayerInfo**(`userId: int64`, `userName: string`, `displayName: string`, `membershipType: MembershipType`, `isUnder13: bool`, `hasRobloxSubscription: bool = false`, `ageCheckedStatus: AgeCheckStatus = Unchecked`) -> `null`
- **TeamChat**(`message: string`) -> `null`
- **UnbanAsync**(`config: Dictionary`) -> `null` [Yields]
- **WhisperChat**(`message: string`, `player: Instance`) -> `null`
- **getPlayers**() -> `Instances` [Deprecated]
- **playerFromCharacter**(`character: Model`) -> `Player` [Deprecated]
- **players**() -> `Instances` [Deprecated]

## Events

- **FriendRequestEvent**(`player: Player`, `player: Player`, `friendRequestEvent: FriendRequestEvent`)
- **PlayerAdded**(`player: Player`)
- **PlayerChatted**(`chatType: PlayerChatType`, `player: Player`, `message: string`, `targetPlayer: Player`)
- **PlayerConnecting**(`player: Player`)
- **PlayerDisconnecting**(`player: Player`)
- **PlayerMembershipChanged**(`player: Player`)
- **PlayerRejoining**(`player: Player`)
- **PlayerRemoving**(`player: Player`, `reason: PlayerExitReason`)
- **PromptAgeCheckRequested**(`player: Player`)
- **UserSubscriptionStatusChanged**(`user: Player`, `subscriptionId: string`)
