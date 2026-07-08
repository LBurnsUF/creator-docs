---
title: FriendPages
type: class
superclass: Pages
tags: [NotCreatable, NotReplicated]
---

# FriendPages

A special version of `Class.Pages` that contains information about a player's
friends.

**Inherits from:** `Class.Pages` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

FriendPages is a special version of `Class.Pages` returned by
`Class.Players:GetFriendsAsync()`. The items contained within include
information about a player's friends and have the following structure:

<table>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
<tr>
<td><code>DisplayName</code></td>
<td>string</td>
<td>The current display name of the friend.</td>
</tr>
<tr>
<td><code>Id</code></td>
<td>int64</td>
<td>The user ID of the friend.</td>
</tr>
<tr>
<td><code>Username</code></td>
<td>string</td>
<td>The username of the friend.</td>
</tr>
</table>

See the code samples for how to iterate over a player's friends.
