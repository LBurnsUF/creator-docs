---
title: EditableImage
type: class
superclass: Object
tags: [NotCreatable]
---

# EditableImage

**Inherits**: Object

**Tags**: NotCreatable

## Properties

- **Size**: `Vector2` [ReadOnly] [NotReplicated]

## Methods

- **Destroy**() -> `null`
- **DrawCircle**(`center: Vector2`, `radius: int`, `color: Color3`, `transparency: float`, `combineType: ImageCombineType`, `antiAliasing: AntiAliasing = Enabled`) -> `null`
- **DrawImage**(`position: Vector2`, `image: EditableImage`, `combineType: ImageCombineType`) -> `null`
- **DrawImageProjected**(`mesh: EditableMesh`, `projection: Dictionary`, `brushConfig: Dictionary`) -> `null`
- **DrawImageTransformed**(`position: Vector2`, `scale: Vector2`, `rotation: float`, `image: EditableImage`, `options: Dictionary?`) -> `null`
- **DrawLine**(`p1: Vector2`, `p2: Vector2`, `color: Color3`, `transparency: float`, `combineType: ImageCombineType`, `antiAliasing: AntiAliasing = Enabled`) -> `null`
- **DrawRectangle**(`position: Vector2`, `size: Vector2`, `color: Color3`, `transparency: float`, `combineType: ImageCombineType`) -> `null`
- **DrawTriangle**(`p1: Vector2`, `p2: Vector2`, `p3: Vector2`, `color: Color3`, `transparency: float`) -> `null`
- **ReadPixelsBuffer**(`position: Vector2`, `size: Vector2`) -> `buffer` [CustomLuaState]
- **WritePixelsBuffer**(`position: Vector2`, `size: Vector2`, `buffer: buffer`) -> `null` [CustomLuaState]
