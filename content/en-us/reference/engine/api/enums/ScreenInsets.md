---
title: ScreenInsets
type: enum
---

# `Enum.ScreenInsets`

Insets associated with various screen safe areas.

This enum specifies screen edge insets that are associated with a particular
screen safe area. The insets are relative to the **fullscreen area**, meaning
the rectangular region that encompasses all visible pixels on the screen.

<img src="../../../assets/engine-api/enums/ScreenInsets/Inset-Regions-All.png" width="840" alt="Mobile device screen showing inset regions." />

The `Enum.ScreenInsets` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ScreenInsets.None` | 0 | No insets are added to the fullscreen area. This mode may result in UI that is obscured or completel |
| `Enum.ScreenInsets.DeviceSafeInsets` | 1 | Device safe area insets are added to the fullscreen area. The resulting area is guaranteed to not be |
| `Enum.ScreenInsets.CoreUISafeInsets` | 2 | Core UI insets are added to the `DeviceSafeInsets` area, resulting in an area guaranteed to be unobs |
| `Enum.ScreenInsets.TopbarSafeInsets` | 3 | Top bar safe area insets are added to the `DeviceSafeInsets` area, resulting in an area guaranteed t |
