---
title: WebStreamClient
type: class
superclass: Object
tags: [NotCreatable, NotReplicated]
---

# WebStreamClient

**Inherits**: Object

**Tags**: NotCreatable, NotReplicated

## Properties

- **ConnectionState**: `WebStreamClientState` [ReadOnly] [NotReplicated]

## Methods

- **Close**() -> `null`
- **Send**(`data: string`) -> `null`

## Events

- **Closed**()
- **Error**(`responseStatusCode: int`, `errorMessage: string`)
- **MessageReceived**(`message: string`)
- **Opened**(`responseStatusCode: int`, `headers: string`)
