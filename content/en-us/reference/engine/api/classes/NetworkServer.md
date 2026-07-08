---
title: NetworkServer
type: class
superclass: NetworkPeer
tags: [NotCreatable, Service, NotReplicated]
---

# NetworkServer

**Inherits from:** `Class.NetworkPeer` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

The `Class.NetworkServer` stores all the `Class.NetworkReplicator` in the game
and handles all connections. `Class.NetworkPeer:SetOutgoingKBPSLimit()` can be
used to imitate latency while using Start Server.

## Methods

### `Class.NetworkServer:EncryptStringForPlayerId`

``EncryptStringForPlayerId(toEncrypt: `string`, playerId: `int64`)`` -> `string`
