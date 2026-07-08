---
title: MessageType
type: enum
---

# `Enum.MessageType`

Message category and severity level.

A message can be a simple diagnostic or a sign of a system instability or
failure. The channel that the message appears in indicates its severity. The
MessageType indicates which channel the message displays in.

The `Enum.MessageType` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.MessageType.MessageOutput` | 0 | The message is from the standard output channel. |
| `Enum.MessageType.MessageInfo` | 1 | The message is from the information channel. |
| `Enum.MessageType.MessageWarning` | 2 | The message is from the warning channel. |
| `Enum.MessageType.MessageError` | 3 | The message is from the error channel. |
