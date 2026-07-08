---
title: VRService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# VRService

Service responsible for handling interactions between Roblox and Virtual
Reality (VR).

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

**VRService** is responsible for handling interactions between Roblox and
Virtual Reality (VR). Its methods, properties, and events help you provide the
best experience for end users seeking to experience Roblox on VR devices.

See [VR Guidelines](../../../production/publishing/vr-guidelines.md) for more
information on publishing an experience for VR devices.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.VRService.AutomaticScaling` | `Enum.VRScaling` |  |
| `Class.VRService.AvatarGestures` | `bool` |  |
| `Class.VRService.ControllerModels` | `Enum.VRControllerModelMode` |  |
| `Class.VRService.DidPointerHit` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.VRService.FadeOutViewOnCollision` | `bool` |  |
| `Class.VRService.GuiInputUserCFrame` | `Enum.UserCFrame` | [NotReplicated] |
| `Class.VRService.LaserDistance` | `float` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.VRService.LaserPointer` | `Enum.VRLaserPointerMode` |  |
| `Class.VRService.PointerHitCFrame` | `Datatype.CFrame` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.VRService.QuestASWState` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.VRService.QuestDisplayRefreshRate` | `float` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.VRService.ThirdPersonFollowCamEnabled` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.VRService.VRDeviceAvailable` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.VRService.VRDeviceName` | `string` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.VRService.VREnabled` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.VRService.VRSessionState` | `Enum.VRSessionState` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |

## Methods

### `Class.VRService:GetTouchpadMode`

``GetTouchpadMode(pad: `Enum.VRTouchpad`)`` -> `Enum.VRTouchpadMode`

### `Class.VRService:GetUserCFrame`

``GetUserCFrame(type: `Enum.UserCFrame`)`` -> `Datatype.CFrame`

### `Class.VRService:GetUserCFrameEnabled`

``GetUserCFrameEnabled(type: `Enum.UserCFrame`)`` -> `bool`

### `Class.VRService:IsMaquettes`

``IsMaquettes()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.VRService:IsVRAppBuild`

``IsVRAppBuild()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.VRService:RecenterUserHeadCFrame`

``RecenterUserHeadCFrame()`` -> `null`

### `Class.VRService:RequestNavigation`

``RequestNavigation(cframe: `Datatype.CFrame`, inputUserCFrame: `Enum.UserCFrame`)`` -> `null`

### `Class.VRService:SetTouchpadMode`

``SetTouchpadMode(pad: `Enum.VRTouchpad`, mode: `Enum.VRTouchpadMode`)`` -> `null`

## Events

### `Class.VRService.LaserPointerTriggered`

Fires with: (input: `Class.InputObject`)

### `Class.VRService.NavigationRequested`

Fires with: (cframe: `Datatype.CFrame`, inputUserCFrame: `Enum.UserCFrame`)

### `Class.VRService.TouchpadModeChanged`

Fires with: (pad: `Enum.VRTouchpad`, mode: `Enum.VRTouchpadMode`)

### `Class.VRService.UserCFrameChanged`

Fires with: (type: `Enum.UserCFrame`, value: `Datatype.CFrame`)

### `Class.VRService.UserCFrameEnabled`

Fires with: (type: `Enum.UserCFrame`, enabled: `bool`)
