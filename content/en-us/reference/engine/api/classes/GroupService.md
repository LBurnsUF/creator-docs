---
title: GroupService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# GroupService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.GroupService:GetAlliesAsync`

``GetAlliesAsync(groupId: `int64`)`` → `Class.StandardPages`
  [Yields]

### `Class.GroupService:GetEnemiesAsync`

``GetEnemiesAsync(groupId: `int64`)`` → `Class.StandardPages`
  [Yields]

### `Class.GroupService:GetGroupInfoAsync`

``GetGroupInfoAsync(groupId: `int64`)`` → `Variant`
  [Yields]

### `Class.GroupService:GetGroupsAsync`

``GetGroupsAsync(userId: `Datatype.User`)`` → `Array`
  [Yields]

### `Class.GroupService:GetRolesInGroupAsync`

``GetRolesInGroupAsync(userId: `Datatype.User`, groupId: `int64`)`` → `Variant`
  [Yields]

### `Class.GroupService:PromptJoinAsync`

``PromptJoinAsync(groupId: `int64`)`` → `Enum.GroupMembershipStatus`
  [Yields]

### `Class.GroupService:PromptJoinCompleted`

``PromptJoinCompleted(groupId: `int64`, success: `bool`, groupMembershipStatus: `Enum.GroupMembershipStatus`, errorMessage: `string`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.GroupService.ShowJoinPrompt`

Fires with: (groupId: `int64`)
