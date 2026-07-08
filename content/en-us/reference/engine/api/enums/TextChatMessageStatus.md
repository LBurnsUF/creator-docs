---
title: TextChatMessageStatus
type: enum
---

# `Enum.TextChatMessageStatus`

Indicates the status of a `Class.TextChatMessage`.

Indicates the status of a `Class.TextChatMessage`.

The `Enum.TextChatMessageStatus` enum has 9 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.TextChatMessageStatus.Unknown` | 1 | Generic failed status for any other `Class.TextChannel:SendAsync()` failures. |
| `Enum.TextChatMessageStatus.Success` | 2 | Message has no issues. |
| `Enum.TextChatMessageStatus.Sending` | 3 | Message is sending. |
| `Enum.TextChatMessageStatus.TextFilterFailed` | 4 | Text filter failed to process the message. |
| `Enum.TextChatMessageStatus.Floodchecked` | 5 | Message is from a user sending messages too frequently. |
| `Enum.TextChatMessageStatus.InvalidPrivacySettings` | 6 | Message can't be sent because of the user's chat privacy settings. |
| `Enum.TextChatMessageStatus.InvalidTextChannelPermissions` | 7 | Message's `Class.TextSource` is either not in the intended `Class.TextChannel` or `Class.TextSource. |
| `Enum.TextChatMessageStatus.MessageTooLong` | 8 | Message is too long. |
| `Enum.TextChatMessageStatus.ModerationTimeout` | 9 |  |
