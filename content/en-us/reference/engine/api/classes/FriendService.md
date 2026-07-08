---
title: FriendService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# FriendService

An internal service which is used to send, cancel, accept and decline friend
requests in-game.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

A service which is used to send, cancel, accept and decline friend requests
in-game. It is primarily used by the PlayerListScript to send friend requests
with the leaderboard.

## Methods

### `Class.FriendService:GetPlatformFriends`

``GetPlatformFriends()`` -> `Array`
  [Yields] {security: RobloxScriptSecurity}

## Events

### `Class.FriendService.FriendsUpdated`

Fires with: (friendData: `Array`)
