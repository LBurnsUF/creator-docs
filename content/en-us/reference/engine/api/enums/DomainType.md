---
title: DomainType
type: enum
---

# `Enum.DomainType`

Specifies the type of domain that a `Datatype.User` is scoped to.

The **DomainType** enum describes the kind of domain in which a domain user ID
is unique. It is used by the `Datatype.User` data type to identify whether the
user's ID belongs to an experience or an OAuth application.

The `Enum.DomainType` enum has 2 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.DomainType.EXPERIENCE` | 1 | The user ID is scoped to a specific experience (universe). |
| `Enum.DomainType.OAUTH` | 3 | The user ID is scoped to a specific OAuth application. |
