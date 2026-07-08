---
title: VirtualUser
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# VirtualUser

VirtualUser is a service that allows you to record the inputs of a user, and
then play it back to a limited extent.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

VirtualUser is a service that allows you to record the inputs of a user, and
then play it back to a limited extent. This service hasn't been maintained in
several years, so it doesn't work very well anymore.

## Methods

### `Class.VirtualUser:Button1Down`

``Button1Down(position: `Datatype.Vector2`, camera: `Datatype.CFrame`)`` -> `null`
   {security: LocalUserSecurity}

### `Class.VirtualUser:Button1Up`

``Button1Up(position: `Datatype.Vector2`, camera: `Datatype.CFrame`)`` -> `null`
   {security: LocalUserSecurity}

### `Class.VirtualUser:Button2Down`

``Button2Down(position: `Datatype.Vector2`, camera: `Datatype.CFrame`)`` -> `null`
   {security: LocalUserSecurity}

### `Class.VirtualUser:Button2Up`

``Button2Up(position: `Datatype.Vector2`, camera: `Datatype.CFrame`)`` -> `null`
   {security: LocalUserSecurity}

### `Class.VirtualUser:CaptureController`

``CaptureController()`` -> `null`
   {security: LocalUserSecurity}

### `Class.VirtualUser:ClickButton1`

``ClickButton1(position: `Datatype.Vector2`, camera: `Datatype.CFrame`)`` -> `null`
   {security: LocalUserSecurity}

### `Class.VirtualUser:ClickButton2`

``ClickButton2(position: `Datatype.Vector2`, camera: `Datatype.CFrame`)`` -> `null`
   {security: LocalUserSecurity}

### `Class.VirtualUser:MoveMouse`

``MoveMouse(position: `Datatype.Vector2`, camera: `Datatype.CFrame`)`` -> `null`
   {security: LocalUserSecurity}

### `Class.VirtualUser:SetKeyDown`

``SetKeyDown(key: `string`)`` -> `null`
   {security: LocalUserSecurity}

### `Class.VirtualUser:SetKeyUp`

``SetKeyUp(key: `string`)`` -> `null`
   {security: LocalUserSecurity}

### `Class.VirtualUser:StartRecording`

``StartRecording()`` -> `null`
   {security: LocalUserSecurity}

### `Class.VirtualUser:StopRecording`

``StopRecording()`` -> `string`
   {security: LocalUserSecurity}

### `Class.VirtualUser:TypeKey`

``TypeKey(key: `string`)`` -> `null`
   {security: LocalUserSecurity}
