---
title: ServerScriptService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ServerScriptService

A container service for server-only `Class.Script` objects.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

**ServerScriptService** is a container service for `Class.Script`,
`Class.ModuleScript` and other scripting-related assets that are only meant
for server use. The contents are never replicated to player clients at all,
which allows for a secure storage of important game logic. Script objects will
run if they are within this service and not
`Class.BaseScript.Disabled|Disabled`.

This service houses just one property,
`Class.ServerScriptService.LoadStringEnabled|LoadStringEnabled`, which
determines whether the `loadstring` function in Luau is enabled. It's
recommended to keep this disabled for security reasons, as misusing this
function can lead to remote code execution vulnerabilities.

Scripts running in ServerScriptService may need access to various other assets
which are not scripting-related, such as prefabricated models to be
`Class.Instance:Clone()|cloned`. Such assets should go in
`Class.ServerStorage`, which behaves similarly to this service except that
`Class.Script` objects will not run even if they are not
`Class.BaseScript.Disabled|Disabled`. Assets and `Class.ModuleScript` that are
useful to both the server and clients should go in `Class.ReplicatedStorage`
instead. Finally, you can further organize objects within this service through
the use of `Class.Folder|Folders` without affecting the way it behaves.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ServerScriptService.LoadStringEnabled` | `bool` | [NotReplicated] [NotScriptable] |
