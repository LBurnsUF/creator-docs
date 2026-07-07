---
title: WebSocketClient
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# WebSocketClient

**Inherits**: Instance > Object

**Tags**: NotCreatable, NotReplicated

## Properties

- **ConnectionState**: `WebSocketState` [ReadOnly] [NotReplicated]

## Methods

- **Close**() -> `null`
- **Send**(`data: string`) -> `null`

## Events

- **Closed**()
- **MessageReceived**(`data: string`)
- **Opened**()
