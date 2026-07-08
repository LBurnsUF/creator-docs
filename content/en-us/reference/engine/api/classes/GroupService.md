---
title: GroupService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# GroupService

GroupService is a service that allows developers to fetch information about a
Roblox group from within a game.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

`GroupService` is a service that allows developers to fetch information about
a Roblox group from within a game.

Basic information on the group, including its name, description, owner, roles
and emblem can be fetched using `Class.GroupService:GetGroupInfoAsync()`.
Lists of a group's allies and enemies can be fetched using
`Class.GroupService:GetAlliesAsync()` and
`Class.GroupService:GetEnemiesAsync()`.

`GroupService` can also be used to fetch a list of groups a player is a member
of, using `Class.GroupService:GetGroupsAsync()`. If you wish to verify if a
player is in a group, use the `Class.Player:IsInGroupAsync()` method rather
than `Class.GroupService:GetGroupsAsync()`.

The service has a number of useful applications, such as detecting if a player
is an ally or enemy upon joining the game, or prompting a player to join a
group using the `Class.GroupService:PromptJoinAsync()` method.

## Methods

### `Class.GroupService:GetAlliesAsync`

``GetAlliesAsync(groupId: `int64`)`` -> `Class.StandardPages`
  [Yields]

### `Class.GroupService:GetEnemiesAsync`

``GetEnemiesAsync(groupId: `int64`)`` -> `Class.StandardPages`
  [Yields]

### `Class.GroupService:GetGroupInfoAsync`

``GetGroupInfoAsync(groupId: `int64`)`` -> `Variant`
  [Yields]

### `Class.GroupService:GetGroupsAsync`

``GetGroupsAsync(userId: `Datatype.User`)`` -> `Array`
  [Yields]

### `Class.GroupService:GetRolesInGroupAsync`

``GetRolesInGroupAsync(userId: `Datatype.User`, groupId: `int64`)`` -> `Variant`
  [Yields]

### `Class.GroupService:PromptJoinAsync`

``PromptJoinAsync(groupId: `int64`)`` -> `Enum.GroupMembershipStatus`
  [Yields]

### `Class.GroupService:PromptJoinCompleted`

``PromptJoinCompleted(groupId: `int64`, success: `bool`, groupMembershipStatus: `Enum.GroupMembershipStatus`, errorMessage: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.GroupService.ShowJoinPrompt`

Fires with: (groupId: `int64`)
