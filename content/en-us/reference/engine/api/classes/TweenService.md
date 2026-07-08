---
title: TweenService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# TweenService

Used to create `Class.Tween|Tweens` which interpolate, or tween, the
properties of instances.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

`Class.TweenService` is used to create `Class.Tween|Tweens` which interpolate,
or tween, the properties of instances. `Class.Tween|Tweens` can be used on any
object with compatible property types, including:

- [number](../../../luau/numbers.md)
- [boolean](../../../luau/booleans.md)
- `Datatype.CFrame`
- `Datatype.Rect`
- `Datatype.Color3`
- `Datatype.UDim`
- `Datatype.UDim2`
- `Datatype.Vector2`
- `Datatype.Vector2int16`
- `Datatype.Vector3`
- `Datatype.EnumItem`

`Class.TweenService:Create()`, the primary constructor function, takes
`Datatype.TweenInfo` specifications about the tween and generates the
`Class.Tween` object which can then be used to play the tween.

Note that `Class.Tween|Tweens` can interpolate multiple properties at the same
time, but they must not be interpolating the same property. If two tweens
attempt to modify the same property, the initial tween will be cancelled and
overwritten by the most recent tween.

## Methods

### `Class.TweenService:Create`

``Create(instance: `Class.Instance`, tweenInfo: `Datatype.TweenInfo`, propertyTable: `Dictionary`)`` -> `Class.Tween`

### `Class.TweenService:GetValue`

``GetValue(alpha: `float`, easingStyle: `Enum.EasingStyle`, easingDirection: `Enum.EasingDirection`)`` -> `float`

### `Class.TweenService:SmoothDamp`

``SmoothDamp(current: `Variant`, target: `Variant`, velocity: `Variant`, smoothTime: `float`, maxSpeed: `float?`, dt: `float?`)`` -> `[{'Category': 'Group', 'Name': 'Variant'}, {'Category': 'Group', 'Name': 'Variant'}]`
