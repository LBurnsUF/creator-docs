---
title: EditableImage
type: class
superclass: Object
tags: [NotCreatable]
---

# EditableImage

Object which allows for the runtime creation and manipulation of images.

**Inherits from:** `Class.Object`

**Tags:** [NotCreatable]

## Description

`EditableImage` allows for the runtime creation and manipulation of images.

To create a blank `EditableImage`, use
`Class.AssetService:CreateEditableImage()`. To create an `EditableImage` from
an existing image, use `Class.AssetService:CreateEditableImageAsync()`.

`EditableImage` can be used in any `Datatype.Content` property which takes an
image, such as `Class.ImageLabel.ImageContent` or
`Class.MeshPart.TextureContent`. This is done by setting the content property
to `Datatype.Content.fromObject(editableImage)`.

The `EditableImage` coordinate system is relative to the top left of the
image:

- Top-left: `(0, 0)`
- Bottom-right: `(Size.X - 1, Size.Y - 1)`

When you use `Class.AssetService:PromptCreateAssetAsync()` to publish an
object that has a `Datatype.Content` property which references an
`EditableImage`, the editable image is published as an image and the property
is set to a new asset ID.

#### Update Limitations

Only a single `EditableImage` can be updated per frame on the display side.
For example, if you update three `EditableImage` objects which are currently
being displayed, it will take three frames for all of them to be updated.

#### Enabling for Published Experiences

For security purposes, using `EditableImage` fails by default for published
experiences. To enable usage, you must be 13+ age verified and ID verified.
After you are verified, open Studio's
[Experience Settings](../../../studio/experience-settings.md), select
**Security**, and enable the **Allow Mesh&nbsp;&#47; Image APIs** toggle.

#### Permissions

To prevent misuse, `Class.AssetService:CreateEditableImageAsync()` only allows
you to load and edit image assets if any of the following is true:

- Owned by or explicitly shared with the experience owner.
- Owned by or explicitly shared with the logged in Studio user.
- Owned by or explicitly shared with the logged in player if the
  `EditableImage` is on the client side.
- Owned by a group where the experience owner, Studio user, or player has a
  role with permission to edit the group's assets. See
  [Roles and permissions](../../../projects/groups.md#roles-and-permissions)
  for more information.

See [Grant permissions](../../../projects/assets/privacy.md#grant-permissions)
to learn how to share assets with users or groups.

The APIs throw an error if they are used to load an asset that does not meet
the criteria above.

#### Memory Limits

Editable assets are currently expensive for memory usage. To minimize its
impact on client performance, `EditableImage` has strict client-side memory
budgets, although the server, Studio, and plugins operate with unlimited
memory. Linking one `Class.EditableImage` to multiple image-related
`Datatype.Content` data types (multi-referencing) can help with memory
optimization.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.EditableImage.Size` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.EditableImage:Destroy`

``Destroy()`` -> `null`

### `Class.EditableImage:DrawCircle`

``DrawCircle(center: `Datatype.Vector2`, radius: `int`, color: `Datatype.Color3`, transparency: `float`, combineType: `Enum.ImageCombineType`, antiAliasing: `Enum.AntiAliasing`)`` -> `null`

### `Class.EditableImage:DrawImage`

``DrawImage(position: `Datatype.Vector2`, image: `Class.EditableImage`, combineType: `Enum.ImageCombineType`)`` -> `null`

### `Class.EditableImage:DrawImageProjected`

``DrawImageProjected(mesh: `Class.EditableMesh`, projection: `Dictionary`, brushConfig: `Dictionary`)`` -> `null`

### `Class.EditableImage:DrawImageTransformed`

``DrawImageTransformed(position: `Datatype.Vector2`, scale: `Datatype.Vector2`, rotation: `float`, image: `Class.EditableImage`, options: `Dictionary?`)`` -> `null`

### `Class.EditableImage:DrawLine`

``DrawLine(p1: `Datatype.Vector2`, p2: `Datatype.Vector2`, color: `Datatype.Color3`, transparency: `float`, combineType: `Enum.ImageCombineType`, antiAliasing: `Enum.AntiAliasing`)`` -> `null`

### `Class.EditableImage:DrawRectangle`

``DrawRectangle(position: `Datatype.Vector2`, size: `Datatype.Vector2`, color: `Datatype.Color3`, transparency: `float`, combineType: `Enum.ImageCombineType`)`` -> `null`

### `Class.EditableImage:DrawTriangle`

``DrawTriangle(p1: `Datatype.Vector2`, p2: `Datatype.Vector2`, p3: `Datatype.Vector2`, color: `Datatype.Color3`, transparency: `float`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.EditableImage:ReadPixelsBuffer`

``ReadPixelsBuffer(position: `Datatype.Vector2`, size: `Datatype.Vector2`)`` -> `Datatype.buffer`
  [CustomLuaState]

### `Class.EditableImage:WritePixelsBuffer`

``WritePixelsBuffer(position: `Datatype.Vector2`, size: `Datatype.Vector2`, buffer: `Datatype.buffer`)`` -> `null`
  [CustomLuaState]
