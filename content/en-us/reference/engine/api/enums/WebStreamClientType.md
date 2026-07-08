---
title: WebStreamClientType
type: enum
---

# `Enum.WebStreamClientType`

Specifies what type of streaming to use when creating a
`Class.WebStreamClient`.

Specifies what type of streaming to use when creating a
`Class.WebStreamClient`.

The `Enum.WebStreamClientType` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.WebStreamClientType.SSE` | 0 | Traditional Server-Sent Events (SSE) client. Requires `text/event-stream` to be returned in the `Con |
| `Enum.WebStreamClientType.RawStream` | 1 | General purpose HTTP streaming client. It can connect to any server that provides streaming data tra |
| `Enum.WebStreamClientType.WebSocket` | 2 | [WebSocket](https://en.wikipedia.org/wiki/WebSocket) client that provides a bidirectional communicat |
