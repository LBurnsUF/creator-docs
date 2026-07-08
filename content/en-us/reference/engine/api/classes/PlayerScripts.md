---
title: PlayerScripts
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# PlayerScripts

A container for client-side scripts to be run inside `Class.Player` objects
within the `Class.Players` service.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

`PlayerScripts` is a container object located inside `Class.Player` objects
within the `Class.Players` service. It is created automatically when a player
joins the game and its main purpose is to contain client scripts copied from
the `Class.StarterPlayerScripts` container within the `Class.StarterPlayer`
service.

Unlike the `Class.Backpack` and `Class.PlayerGui` containers, the
`PlayerScripts` container is not accessible to the server and server‑side
`Class.Script` objects will not run when parented to `PlayerScripts`.

## Methods

### `Class.PlayerScripts:ClearComputerCameraMovementModes`

``ClearComputerCameraMovementModes()`` -> `null`

### `Class.PlayerScripts:ClearComputerMovementModes`

``ClearComputerMovementModes()`` -> `null`

### `Class.PlayerScripts:ClearTouchCameraMovementModes`

``ClearTouchCameraMovementModes()`` -> `null`

### `Class.PlayerScripts:ClearTouchMovementModes`

``ClearTouchMovementModes()`` -> `null`

### `Class.PlayerScripts:GetRegisteredComputerCameraMovementModes`

``GetRegisteredComputerCameraMovementModes()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.PlayerScripts:GetRegisteredComputerMovementModes`

``GetRegisteredComputerMovementModes()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.PlayerScripts:GetRegisteredTouchCameraMovementModes`

``GetRegisteredTouchCameraMovementModes()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.PlayerScripts:GetRegisteredTouchMovementModes`

``GetRegisteredTouchMovementModes()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.PlayerScripts:RegisterComputerCameraMovementMode`

``RegisterComputerCameraMovementMode(cameraMovementMode: `Enum.ComputerCameraMovementMode`)`` -> `null`

### `Class.PlayerScripts:RegisterComputerMovementMode`

``RegisterComputerMovementMode(movementMode: `Enum.ComputerMovementMode`)`` -> `null`

### `Class.PlayerScripts:RegisterTouchCameraMovementMode`

``RegisterTouchCameraMovementMode(cameraMovementMode: `Enum.TouchCameraMovementMode`)`` -> `null`

### `Class.PlayerScripts:RegisterTouchMovementMode`

``RegisterTouchMovementMode(movementMode: `Enum.TouchMovementMode`)`` -> `null`

## Events

### `Class.PlayerScripts.ComputerCameraMovementModeRegistered`

Fires with: ()

### `Class.PlayerScripts.ComputerMovementModeRegistered`

Fires with: ()

### `Class.PlayerScripts.TouchCameraMovementModeRegistered`

Fires with: ()

### `Class.PlayerScripts.TouchMovementModeRegistered`

Fires with: ()
