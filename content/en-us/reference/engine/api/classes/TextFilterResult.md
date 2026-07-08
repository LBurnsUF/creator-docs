---
title: TextFilterResult
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# TextFilterResult

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

Represents the result of a call to `Class.TextService:FilterStringAsync()`.
Used to distribute a filtered string accordingly.

## Methods

### `Class.TextFilterResult:GetChatForUserAsync`

``GetChatForUserAsync(toUserId: `int64`)`` -> `string`
  [Yields] [Deprecated]

### `Class.TextFilterResult:GetNonChatStringForBroadcastAsync`

``GetNonChatStringForBroadcastAsync()`` -> `string`
  [Yields]

### `Class.TextFilterResult:GetNonChatStringForUserAsync`

``GetNonChatStringForUserAsync(toUserId: `int64`)`` -> `string`
  [Yields]
