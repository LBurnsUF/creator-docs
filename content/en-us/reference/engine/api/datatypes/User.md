---
title: User
type: datatype
---

# `Datatype.User`

Represents a user's domain-scoped identity within a specific domain.

## Description

The **User** data type represents a user's scoped identity within a specific
domain, such as an experience or OAuth application. It encapsulates a domain
user ID alongside the domain metadata that uniquely identifies that user
within that domain.

Unlike a numeric user ID alone, a `Datatype.User` value carries its domain
context, making it unambiguous across experiences and apps. It is the standard
identifier for referencing users in new experience code and is available from
`Class.Player.User`.

#### Domain User IDs

User IDs on Roblox are **domain-scoped**: a single account has a unique domain
user ID for each experience or app it interacts with. This ensures that user
activity in one experience cannot be correlated with activity in another by a
third party using the user ID alone.

A domain user ID is an integer that is unique within a given domain
(identified by `Enum.DomainType` and domain ID). Domain user IDs are
guaranteed not to collide with existing global user IDs.

#### Serialization

`Datatype.User` supports round-trip string serialization via
`Datatype.User:ToString()|ToString()` and
`Datatype.User.fromString()|fromString()`. A `Datatype.User` serialized with
`ToString()` and deserialized with `fromString()` produces an identical value.
The encoded string is stable, URL-safe, and compact. Use it when persisting or
transmitting user identity across systems.

```lua
-- Serialize
local encoded = player.User:ToString()

-- Deserialize
local user = User.fromString(encoded)
```

#### Users vs. Players

A `Datatype.User` represents persistent identity, not live server presence. It
can reference any account in the domain, whether or not that user is currently
connected. Use `Class.Player` when you need the in-server instance.

## Constructors

### `User.fromId`

Creates a new `Datatype.User` from the given domain user ID, using the current
experience as the domain. The ID must be a valid domain user ID (above the
global user ID range).

```lua
local user = User.fromId(domainUserId)
print(user.Id)         -- domainUserId
print(user.DomainType) -- Enum.DomainType.EXPERIENCE
```

**Parameters:**

- `domainUserId`: `int64`

### `User.fromString`

Deserializes a `Datatype.User` from a string previously produced by
`Datatype.User:ToString()|ToString()`.

```lua
local encoded = player.User:ToString()
local restored = User.fromString(encoded)
print(restored.Id == player.User.Id) -- true
```

**Parameters:**

- `userString`: `string`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `User.Id` | `int64` | The domain user ID, unique within this domain. |
| `User.DomainType` | `DomainType` | The type of domain that this domain user ID belongs to. |
| `User.DomainId` | `int64` | The identifier of the specific domain instance. |

## Methods

### `User:ToString`

Serializes this `Datatype.User` into a string that encodes the domain
type, domain ID, and domain user ID. The result is stable, URL-safe, and
compact. Use this when storing or transmitting user identity.

The string can be converted back to a `Datatype.User` via
`Datatype.User.fromString()|fromString()`.

```lua
local encoded = player.User:ToString()
-- Store in a data store, send over a remote, etc.
DataStore:SetAsync("last_visitor", encoded)
```

## API Usage (45 locations)

### Used as Property Type

- `Class.Player.User`

### Used as Parameter Type

- `Class.AnimationClipProvider:GetAnimations` (parameter `userId`)
- `Class.AnimationClipProvider:GetAnimationsAsync` (parameter `userId`)
- `Class.BadgeService:AwardBadge` (parameter `userId`)
- `Class.BadgeService:AwardBadgeAsync` (parameter `userId`)
- `Class.BadgeService:CheckUserBadgesAsync` (parameter `userId`)
- `Class.BadgeService:UserHasBadge` (parameter `userId`)
- `Class.BadgeService:UserHasBadgeAsync` (parameter `userId`)
- `Class.GroupService:GetGroupsAsync` (parameter `userId`)
- `Class.GroupService:GetRolesInGroupAsync` (parameter `userId`)
- `Class.GuiService:InspectPlayerFromUserId` (parameter `userId`)
- `Class.GuiService:InspectPlayerFromUserIdWithCtx` (parameter `userId`)
- `Class.InsertService:GetUserCategories` (parameter `userId`)
- `Class.InsertService:GetUserSets` (parameter `userId`)
- `Class.KeyframeSequenceProvider:GetAnimations` (parameter `userId`)
- `Class.KeyframeSequenceProvider:GetAnimationsAsync` (parameter `userId`)
- `Class.MarketplaceService:UserOwnsGamePassAsync` (parameter `userId`)
- `Class.Player:IsBestFriendsWith` (parameter `userId`)
- `Class.Player:IsFriendsWith` (parameter `userId`)
- `Class.Player:IsFriendsWithAsync` (parameter `userId`)
- `Class.Player:isFriendsWith` (parameter `userId`)
- `Class.Players:CreateHumanoidModelFromUserId` (parameter `userId`)
- `Class.Players:CreateHumanoidModelFromUserIdAsync` (parameter `userId`)
- `Class.Players:GetBanHistoryAsync` (parameter `userId`)
- `Class.Players:GetCharacterAppearanceAsync` (parameter `userId`)
- `Class.Players:GetCharacterAppearanceInfoAsync` (parameter `userId`)
- `Class.Players:GetFriendsAsync` (parameter `userId`)
- `Class.Players:GetHumanoidDescriptionFromUserId` (parameter `userId`)
- `Class.Players:GetHumanoidDescriptionFromUserIdAsync` (parameter `userId`)
- `Class.Players:GetNameFromUserIdAsync` (parameter `userId`)
- `Class.Players:GetPlayerByUserId` (parameter `userId`)
- `Class.Players:GetProfileConfigurationFromUserIdAsync` (parameter `userId`)
- `Class.Players:GetUserThumbnailAsync` (parameter `userId`)
- `Class.SocialService:CanSendGameInviteAsync` (parameter `recipientId`)
- `Class.TeleportService:GetPlayerPlaceInstanceAsync` (parameter `userId`)
- `Class.TextChannel:AddUserAsync` (parameter `userId`)
- `Class.TextChatService:CanUserChatAsync` (parameter `userId`)
- `Class.TextChatService:CanUsersChatAsync` (parameter `userIdFrom`)
- `Class.TextChatService:CanUsersChatAsync` (parameter `userIdTo`)
- `Class.TextChatService:CanUsersDirectChatAsync` (parameter `requesterUserId`)
- `Class.TextChatService:CanUsersWhisperAsync` (parameter `fromUserId`)
- ...and 3 more

### Used as Return Type

- `Class.UserService:GetUserFromGlobalUserIdAsync`
