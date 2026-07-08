---
title: AssetFetchStatus
type: enum
---

# `Enum.AssetFetchStatus`

The `Enum.AssetFetchStatus` enum has 5 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.AssetFetchStatus.Success` | 0 | The asset loaded successfully. |
| `Enum.AssetFetchStatus.Failure` | 1 | The asset failed to load successfully. Subsequent attempts are likely to fail; there may be somethin |
| `Enum.AssetFetchStatus.None` | 2 | The engine has no information about this asset. The engine never tried to load it. |
| `Enum.AssetFetchStatus.Loading` | 3 | The engine is in the middle of trying to load this asset. |
| `Enum.AssetFetchStatus.TimedOut` | 4 | The engine tried to load this asset but timed out. Future attempts to load may succeed. |
