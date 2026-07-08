---
title: WrapTarget
type: class
superclass: BaseWrap
---

# WrapTarget

The WrapTarget object defines a target. A target is the 3D body with only an
outer surface, or an Outer Cage.

**Inherits from:** `Class.BaseWrap` > `Class.Instance` > `Class.Object`

## Description

The WrapTarget object defines a target. A target is the 3D body with only an
outer surface, or an Outer Cage.

This target, often an Avatar, is what 3D accessories (using WrapLayer) will be
applied to, allowing multiple accessories items to naturally layer over the
source target.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.WrapTarget.Color` | `Datatype.Color3` | [NotReplicated] [NotScriptable] |
| `Class.WrapTarget.DebugMode` | `Enum.WrapTargetDebugMode` | [NotReplicated] [NotScriptable] |
| `Class.WrapTarget.Stiffness` | `float` | [Deprecated] {write: PluginSecurity} |
