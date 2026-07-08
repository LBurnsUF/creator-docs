---
title: ReplicatedFirst
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# ReplicatedFirst

A container whose contents are replicated to all clients (but not back to the
server) first before anything else.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

`ReplicatedFirst` is a container whose contents are replicated to all clients
(but not back to the server) before anything else. It's most commonly used to
store `Class.LocalScript|LocalScripts` and other elements that are essential
for the experience's start such as
[loading screens](../../../players/loading-screens.md).

For objects that do **not** need to be replicated before anything else, use
the `Class.ReplicatedStorage` container instead.

There are some key considerations for running `Class.LocalScript|LocalScripts`
in `ReplicatedFirst`:

- Since its contents replicate before anything else in the experience,
  `Class.LocalScript|LocalScripts` running in `ReplicatedFirst` will need to
  wait for any objects they require to replicate using
  `Class.Instance:WaitForChild()`
- Any objects that are to be used by a `Class.LocalScript` in
  `ReplicatedFirst` should also be parented to `ReplicatedFirst`. Otherwise,
  they may replicate to the client late, yielding the script and negating the
  benefit of initial replication.

## Methods

### `Class.ReplicatedFirst:IsDefaultLoadingGuiRemoved`

``IsDefaultLoadingGuiRemoved()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.ReplicatedFirst:IsFinishedReplicating`

``IsFinishedReplicating()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.ReplicatedFirst:RemoveDefaultLoadingScreen`

``RemoveDefaultLoadingScreen()`` -> `null`

### `Class.ReplicatedFirst:SetDefaultLoadingGuiRemoved`

``SetDefaultLoadingGuiRemoved()`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.ReplicatedFirst.DefaultLoadingGuiRemoved`

Fires with: ()

### `Class.ReplicatedFirst.FinishedReplicating`

Fires with: ()

### `Class.ReplicatedFirst.RemoveDefaultLoadingGuiSignal`

Fires with: ()
