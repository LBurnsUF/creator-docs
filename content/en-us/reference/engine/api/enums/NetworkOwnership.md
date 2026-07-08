---
title: NetworkOwnership
type: enum
---

# `Enum.NetworkOwnership`

Defines how simulation authority is determined for the Network Ownership
Unit/Mechanism this part is attached to.

Defines how to determine which client has ownership of a part for a server
(network).

The `Enum.NetworkOwnership` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.NetworkOwnership.Automatic` | 0 | Network ownership is determined automatically by the server. |
| `Enum.NetworkOwnership.Manual` | 1 | Network ownership is set manually by the developer. |
| `Enum.NetworkOwnership.OnContact` | 2 | The first player to touch a part is given ownership of that part for the server (network). Ownership |
