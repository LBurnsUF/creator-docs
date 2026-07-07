---
title: Lighting
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# Lighting

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.Lighting.Ambient` | `Datatype.Color3` |  |
| `Class.Lighting.Brightness` | `float` |  |
| `Class.Lighting.ClockTime` | `float` | [NotReplicated] |
| `Class.Lighting.ColorShift_Bottom` | `Datatype.Color3` |  |
| `Class.Lighting.ColorShift_Top` | `Datatype.Color3` |  |
| `Class.Lighting.EnvironmentDiffuseScale` | `float` |  |
| `Class.Lighting.EnvironmentSpecularScale` | `float` |  |
| `Class.Lighting.ExposureCompensation` | `float` |  |
| `Class.Lighting.ExtendLightRangeTo120` | `Enum.RolloutState` | [NotScriptable] |
| `Class.Lighting.FogColor` | `Datatype.Color3` |  |
| `Class.Lighting.FogEnd` | `float` |  |
| `Class.Lighting.FogStart` | `float` |  |
| `Class.Lighting.GeographicLatitude` | `float` |  |
| `Class.Lighting.GlobalShadows` | `bool` |  |
| `Class.Lighting.LightingStyle` | `Enum.LightingStyle` |  {write: RobloxScriptSecurity} |
| `Class.Lighting.OutdoorAmbient` | `Datatype.Color3` |  |
| `Class.Lighting.Outlines` | `bool` | [Deprecated] |
| `Class.Lighting.PrioritizeLightingQuality` | `bool` |  {write: RobloxScriptSecurity} |
| `Class.Lighting.ShadowColor` | `Datatype.Color3` | [NotReplicated] [Deprecated] |
| `Class.Lighting.ShadowSoftness` | `float` |  |
| `Class.Lighting.Technology` | `Enum.Technology` |  {security: RobloxScriptSecurity} |
| `Class.Lighting.TimeOfDay` | `string` |  |

## Methods

### `Class.Lighting:GetMinutesAfterMidnight`

``GetMinutesAfterMidnight()`` → `double`

### `Class.Lighting:GetMoonDirection`

``GetMoonDirection()`` → `Datatype.Vector3`

### `Class.Lighting:GetMoonPhase`

``GetMoonPhase()`` → `float`

### `Class.Lighting:GetSunDirection`

``GetSunDirection()`` → `Datatype.Vector3`

### `Class.Lighting:SetMinutesAfterMidnight`

``SetMinutesAfterMidnight(minutes: `double`)`` → `null`

### `Class.Lighting:getMinutesAfterMidnight`

``getMinutesAfterMidnight()`` → `double`
  [Deprecated]

### `Class.Lighting:setMinutesAfterMidnight`

``setMinutesAfterMidnight(minutes: `double`)`` → `null`
  [Deprecated]

## Events

### `Class.Lighting.LightingChanged`

Fires with: (skyChanged: `bool`)
