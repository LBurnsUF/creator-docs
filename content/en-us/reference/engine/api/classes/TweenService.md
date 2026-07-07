---
title: TweenService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# TweenService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.TweenService:Create`

``Create(instance: `Class.Instance`, tweenInfo: `Datatype.TweenInfo`, propertyTable: `Dictionary`)`` → `Class.Tween`

### `Class.TweenService:GetValue`

``GetValue(alpha: `float`, easingStyle: `Enum.EasingStyle`, easingDirection: `Enum.EasingDirection`)`` → `float`

### `Class.TweenService:SmoothDamp`

``SmoothDamp(current: `Variant`, target: `Variant`, velocity: `Variant`, smoothTime: `float`, maxSpeed: `float?`, dt: `float?`)`` → `[{'Category': 'Group', 'Name': 'Variant'}, {'Category': 'Group', 'Name': 'Variant'}]`
