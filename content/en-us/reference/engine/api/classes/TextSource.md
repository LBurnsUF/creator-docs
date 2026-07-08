---
title: TextSource
type: class
superclass: Instance
tags: [NotCreatable]
---

# TextSource

Represents a speaker in a `Class.TextChannel`.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

Represents a speaker in a `Class.TextChannel`.

`Class.TextSource|TextSources` provide details on permissions users have in
`Class.TextChannel|TextChannels`. There may be multiple
`Class.TextSource|TextSources` for a user if that user belongs in multiple
`Class.TextChannel|TextChannels`.

Create `Class.TextSource|TextSources` with `Class.TextChannel:AddUserAsync()`,
which adds a `Class.TextSource` to the `Class.TextChannel` as a descendant.

Remove `Class.TextSource|TextSources` by calling `Class.TextSource.Destroy`.

Name of a `Class.TextSource` is the `Class.Player.DisplayName` of the user
associated with the `Class.TextSource` via `Class.TextSource.UserId`.

To learn more about using TextSources, see
[In-Experience Text Chat](../../../chat/in-experience-text-chat.md).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.TextSource.CanSend` | `bool` |  |
| `Class.TextSource.DisplayName` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.TextSource.UserId` | `int64` | [ReadOnly] [NotReplicated] |
| `Class.TextSource.Username` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
