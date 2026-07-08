---
title: NetworkClient
type: class
superclass: NetworkPeer
tags: [NotCreatable, Service, NotReplicated]
---

# NetworkClient

**Inherits from:** `Class.NetworkPeer` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

This service is responsible for connecting a client to a server.

## Events

### `Class.NetworkClient.ConnectionAccepted`

Fires with: (peer: `string`, replicator: `Class.Instance`)

### `Class.NetworkClient.ConnectionFailed`

Fires with: (peer: `string`, code: `int`)
