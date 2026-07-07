---
title: VideoCaptureService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# VideoCaptureService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **Active**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **CameraID**: `string` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **GetCameraDevices**() -> `Map`

## Events

- **DevicesChanged**()
- **Error**(`cameraid: string`, `errorcode: string`)
- **Started**(`cameraid: string`)
- **Stopped**(`cameraid: string`)
