---
title: SafeAreaCompatibility
type: enum
---

# `Enum.SafeAreaCompatibility`

Describes how descendants of a `Class.ScreenGui` adapt to screens with
cutouts.

This enum describes the automatic compatibility transformations that apply to
descendant "fullscreen" `Class.GuiObject|GuiObjects` of a `Class.ScreenGui` on
displays with screen cutouts.

The `Enum.SafeAreaCompatibility` enum has 2 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.SafeAreaCompatibility.None` | 0 | Do not apply compatibility transformations to any descendants of the `Class.ScreenGui`. |
| `Enum.SafeAreaCompatibility.FullscreenExtension` | 1 | If the total area of any descendant `Class.GuiObject` within the `Class.ScreenGui` (including any ap |
