---
title: ScreenshotHud
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# ScreenshotHud

A 2D user interface that allows users to capture and save screenshots to their
local device.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

The `Class.ScreenshotHud` is a 2D user interface that allows users to capture
and save screenshots to their local device. It consists of the following UI
elements:

- An overlay containing the experience name and Roblox branding. These remain
  on screen when a screenshot is taken, although the experience name can be
  disabled through the `Class.ScreenshotHud.ExperienceNameOverlayEnabled`
  property.
- A camera button that hides all UI except for the overlay and takes a
  screenshot.
- A close button that closes the `Class.ScreenshotHud`.

<img src="../../../assets/engine-api/classes/ScreenshotHud/Diagram.jpg" width="100%" />

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ScreenshotHud.CameraButtonIcon` | `Datatype.ContentId` |  |
| `Class.ScreenshotHud.CameraButtonIconContent` | `Datatype.Content` |  |
| `Class.ScreenshotHud.CameraButtonPosition` | `Datatype.UDim2` |  |
| `Class.ScreenshotHud.CloseButtonPosition` | `Datatype.UDim2` |  |
| `Class.ScreenshotHud.CloseWhenScreenshotTaken` | `bool` |  |
| `Class.ScreenshotHud.ExperienceNameOverlayEnabled` | `bool` | [Hidden] [Deprecated] |
| `Class.ScreenshotHud.HideCoreGuiForCaptures` | `bool` |  |
| `Class.ScreenshotHud.HidePlayerGuiForCaptures` | `bool` |  |
| `Class.ScreenshotHud.OverlayFont` | `Enum.Font` | [Hidden] [Deprecated] |
| `Class.ScreenshotHud.UsernameOverlayEnabled` | `bool` | [Hidden] [Deprecated] |
| `Class.ScreenshotHud.Visible` | `bool` |  |
