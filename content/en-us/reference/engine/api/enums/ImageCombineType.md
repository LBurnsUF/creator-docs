---
title: ImageCombineType
type: enum
---

# `Enum.ImageCombineType`

Enum for determining how two images are combined together.

Enum for determining how two images are combined together.

In all combine operations, **source** refers to the new pixels being drawn and
**destination** refers to the existing pixels in the image being drawn onto.

The `Enum.ImageCombineType` enum has 6 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ImageCombineType.BlendSourceOver` | 1 | Blends pixels from the source with pixels from the destination using source over alpha blending. |
| `Enum.ImageCombineType.Overwrite` | 2 | Overwrites all pixels in the destination image with pixels from the source image. |
| `Enum.ImageCombineType.Add` | 3 | Adds pixels from the source and pixels from the destination together. |
| `Enum.ImageCombineType.Multiply` | 4 | Multiplies pixels from the source and pixels from the destination together. RGBA values are multipli |
| `Enum.ImageCombineType.AlphaBlend` | 5 | Blends pixels from the source with pixels from the destination based on the alpha of the source pixe |
| `Enum.ImageCombineType.NormalMapBlend` | 6 |  |
