---
title: GroupMembershipStatus
type: enum
---

# `Enum.GroupMembershipStatus`

Defines the possible outcomes of the `Class.GroupService:PromptJoinAsync()`
method.

`GroupMembershipStatus` is an enumeration that represents the result of a
player's interaction with the `Class.GroupService:PromptJoinAsync()` method.
It conveys the player's group membership status after the prompt.

The `Enum.GroupMembershipStatus` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.GroupMembershipStatus.None` | 0 | The player chose not to join, cancelled the prompt, or was not eligible to join the group. |
| `Enum.GroupMembershipStatus.Joined` | 1 | The player successfully joined the group during the prompt. |
| `Enum.GroupMembershipStatus.JoinRequestPending` | 2 | The player submitted a request to join the group, or already had a pending join request prior to pro |
| `Enum.GroupMembershipStatus.AlreadyMember` | 3 | The player was already a member of the group. |
