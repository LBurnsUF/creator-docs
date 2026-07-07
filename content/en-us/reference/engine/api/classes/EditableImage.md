---
title: EditableImage
type: class
superclass: Object
tags: [NotCreatable]
---

# EditableImage

**Inherits from:** `Class.Object`

**Tags:** [NotCreatable]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.EditableImage.Size` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.EditableImage:Destroy`

``Destroy()`` → `null`

### `Class.EditableImage:DrawCircle`

``DrawCircle(center: `Datatype.Vector2`, radius: `int`, color: `Datatype.Color3`, transparency: `float`, combineType: `Enum.ImageCombineType`, antiAliasing: `Enum.AntiAliasing`)`` → `null`

### `Class.EditableImage:DrawImage`

``DrawImage(position: `Datatype.Vector2`, image: `Class.EditableImage`, combineType: `Enum.ImageCombineType`)`` → `null`

### `Class.EditableImage:DrawImageProjected`

``DrawImageProjected(mesh: `Class.EditableMesh`, projection: `Dictionary`, brushConfig: `Dictionary`)`` → `null`

### `Class.EditableImage:DrawImageTransformed`

``DrawImageTransformed(position: `Datatype.Vector2`, scale: `Datatype.Vector2`, rotation: `float`, image: `Class.EditableImage`, options: `Dictionary?`)`` → `null`

### `Class.EditableImage:DrawLine`

``DrawLine(p1: `Datatype.Vector2`, p2: `Datatype.Vector2`, color: `Datatype.Color3`, transparency: `float`, combineType: `Enum.ImageCombineType`, antiAliasing: `Enum.AntiAliasing`)`` → `null`

### `Class.EditableImage:DrawRectangle`

``DrawRectangle(position: `Datatype.Vector2`, size: `Datatype.Vector2`, color: `Datatype.Color3`, transparency: `float`, combineType: `Enum.ImageCombineType`)`` → `null`

### `Class.EditableImage:DrawTriangle`

``DrawTriangle(p1: `Datatype.Vector2`, p2: `Datatype.Vector2`, p3: `Datatype.Vector2`, color: `Datatype.Color3`, transparency: `float`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.EditableImage:ReadPixelsBuffer`

``ReadPixelsBuffer(position: `Datatype.Vector2`, size: `Datatype.Vector2`)`` → `Datatype.buffer`
  [CustomLuaState]

### `Class.EditableImage:WritePixelsBuffer`

``WritePixelsBuffer(position: `Datatype.Vector2`, size: `Datatype.Vector2`, buffer: `Datatype.buffer`)`` → `null`
  [CustomLuaState]
