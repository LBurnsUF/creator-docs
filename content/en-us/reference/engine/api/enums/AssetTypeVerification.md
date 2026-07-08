---
title: AssetTypeVerification
type: enum
---

# `Enum.AssetTypeVerification`

Determines the asset type verification mode.

Determines the asset type verification mode used when calling
`Class.Humanoid:ApplyDescriptionAsync()` or
`Class.Players:CreateHumanoidModelFromDescriptionAsync()`. This verification
mode determines if the method will load models or not. Loading models can be
insecure if it's possible for malicious users to trick your game into loading
unexpected models that you own which may include malicious scripts. You should
set this to `Always` unless you want to load non-catalog assets.

The `Enum.AssetTypeVerification` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.AssetTypeVerification.Default` | 1 | Use the default behavior for asset type verification. |
| `Enum.AssetTypeVerification.ClientOnly` | 2 | Only verify asset types on the client. Asset type verification can not be turned off on the client. |
| `Enum.AssetTypeVerification.Always` | 3 | Always verify the asset types to be loaded and disallow loading models. |
