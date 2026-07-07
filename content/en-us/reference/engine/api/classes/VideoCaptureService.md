---
title: VideoCaptureService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# VideoCaptureService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.VideoCaptureService.Active` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.VideoCaptureService.CameraID` | `string` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |

## Methods

### `Class.VideoCaptureService:GetCameraDevices`

``GetCameraDevices()`` → `Map`
   {security: RobloxScriptSecurity}

## Events

### `Class.VideoCaptureService.DevicesChanged`

Fires with: ()

### `Class.VideoCaptureService.Error`

Fires with: (cameraid: `string`, errorcode: `string`)

### `Class.VideoCaptureService.Started`

Fires with: (cameraid: `string`)

### `Class.VideoCaptureService.Stopped`

Fires with: (cameraid: `string`)
