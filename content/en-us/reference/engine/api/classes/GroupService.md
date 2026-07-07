---
title: GroupService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# GroupService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **GetAlliesAsync**(`groupId: int64`) -> `StandardPages` [Yields]
- **GetEnemiesAsync**(`groupId: int64`) -> `StandardPages` [Yields]
- **GetGroupInfoAsync**(`groupId: int64`) -> `Variant` [Yields]
- **GetGroupsAsync**(`userId: User`) -> `Array` [Yields]
- **GetRolesInGroupAsync**(`userId: User`, `groupId: int64`) -> `Variant` [Yields]
- **PromptJoinAsync**(`groupId: int64`) -> `GroupMembershipStatus` [Yields]
- **PromptJoinCompleted**(`groupId: int64`, `success: bool`, `groupMembershipStatus: GroupMembershipStatus`, `errorMessage: string`) -> `null`

## Events

- **ShowJoinPrompt**(`groupId: int64`)
