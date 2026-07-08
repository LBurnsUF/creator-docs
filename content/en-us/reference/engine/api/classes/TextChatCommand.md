---
title: TextChatCommand
type: class
superclass: Instance
---

# TextChatCommand

Represents a text chat command.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

Represents a text chat command. Can be used to create custom text chat
commands when parented to `Class.TextChatService`.

Custom commands can have up to two aliases, and the Triggered event fires when
a user's message matches the value of either the
`Class.TextChatCommand.PrimaryAlias|PrimaryAlias` or
`Class.TextChatCommand.SecondaryAlias|SecondaryAlias`. For an example of
custom commands, see
[Custom text chat commands](../../../chat/examples/custom-text-chat-commands.md).

To learn more about using `Class.TextChatService`, see
[In-experience text chat](../../../chat/in-experience-text-chat.md).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.TextChatCommand.AutocompleteVisible` | `bool` |  |
| `Class.TextChatCommand.Enabled` | `bool` |  |
| `Class.TextChatCommand.PrimaryAlias` | `string` |  |
| `Class.TextChatCommand.SecondaryAlias` | `string` |  |

## Events

### `Class.TextChatCommand.Triggered`

Fires with: (originTextSource: `Class.TextSource`, unfilteredText: `string`)
