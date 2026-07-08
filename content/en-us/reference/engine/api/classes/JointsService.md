---
title: JointsService
type: class
superclass: Instance
tags: [NotCreatable, Service, Deprecated]
---

# JointsService

A service that stores joints created by surface connections.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [Deprecated]

## Description

The JointsService is a service that stores joints created by surface
connections. It also has API available for visualizing surface to surface
contact, and joining surfaces together.

> **Deprecated:** This service has been deprecated in favor of
[constraints](../../../physics/mechanical-constraints.md) which should be used
for surface connections instead

## Methods

### `Class.JointsService:ClearJoinAfterMoveJoints`

``ClearJoinAfterMoveJoints()`` -> `null`

### `Class.JointsService:CreateJoinAfterMoveJoints`

``CreateJoinAfterMoveJoints()`` -> `null`

### `Class.JointsService:SetJoinAfterMoveInstance`

``SetJoinAfterMoveInstance(joinInstance: `Class.Instance`)`` -> `null`

### `Class.JointsService:SetJoinAfterMoveTarget`

``SetJoinAfterMoveTarget(joinTarget: `Class.Instance`)`` -> `null`

### `Class.JointsService:ShowPermissibleJoints`

``ShowPermissibleJoints()`` -> `null`
