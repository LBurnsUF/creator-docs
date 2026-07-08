---
title: WebStreamClientState
type: enum
---

# `Enum.WebStreamClientState`

WebStreamClientState indicates the current state of a WebStreamClient object.

WebStreamClientState indicates the current state of a WebStreamClient object.

The `Enum.WebStreamClientState` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.WebStreamClientState.Connecting` | 0 | The client has sent a request to connect with the server and is waiting for a response. |
| `Enum.WebStreamClientState.Open` | 1 | The client is connected to the server, allowing for data to be streamed between the server and clien |
| `Enum.WebStreamClientState.Error` | 2 | An unrecoverable error has occured while setting up the connection orduring the connection lifetime, |
| `Enum.WebStreamClientState.Closed` | 3 | The connection has run to completion without issues, either closed naturally by the server or manual |
