---
title: VRService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# VRService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **AutomaticScaling**: `VRScaling`
- **AvatarGestures**: `bool`
- **ControllerModels**: `VRControllerModelMode`
- **DidPointerHit**: `bool` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **FadeOutViewOnCollision**: `bool`
- **GuiInputUserCFrame**: `UserCFrame` [NotReplicated]
- **LaserDistance**: `float` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **LaserPointer**: `VRLaserPointerMode`
- **PointerHitCFrame**: `CFrame` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **QuestASWState**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **QuestDisplayRefreshRate**: `float` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **ThirdPersonFollowCamEnabled**: `bool` [ReadOnly] [NotReplicated]
- **VRDeviceAvailable**: `bool` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **VRDeviceName**: `string` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **VREnabled**: `bool` [ReadOnly] [NotReplicated]
- **VRSessionState**: `VRSessionState` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **GetTouchpadMode**(`pad: VRTouchpad`) -> `VRTouchpadMode`
- **GetUserCFrame**(`type: UserCFrame`) -> `CFrame`
- **GetUserCFrameEnabled**(`type: UserCFrame`) -> `bool`
- **IsMaquettes**() -> `bool`
- **IsVRAppBuild**() -> `bool`
- **RecenterUserHeadCFrame**() -> `null`
- **RequestNavigation**(`cframe: CFrame`, `inputUserCFrame: UserCFrame`) -> `null`
- **SetTouchpadMode**(`pad: VRTouchpad`, `mode: VRTouchpadMode`) -> `null`

## Events

- **LaserPointerTriggered**(`input: InputObject`)
- **NavigationRequested**(`cframe: CFrame`, `inputUserCFrame: UserCFrame`)
- **TouchpadModeChanged**(`pad: VRTouchpad`, `mode: VRTouchpadMode`)
- **UserCFrameChanged**(`type: UserCFrame`, `value: CFrame`)
- **UserCFrameEnabled**(`type: UserCFrame`, `enabled: bool`)
