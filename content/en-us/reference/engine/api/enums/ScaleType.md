---
title: ScaleType
type: enum
---

# `Enum.ScaleType`

Determines how an image (of a `Class.ImageLabel` or `Class.ImageButton`) is
scaled.

Determines how an image (of a `Class.ImageLabel` or `Class.ImageButton`) is
scaled.

The `Enum.ScaleType` enum has 5 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ScaleType.Stretch` | 0 | The image is stretched to fit within the element. |
| `Enum.ScaleType.Slice` | 1 | 9-Slice scaling: slice the image into 9 regions and apply different scaling rules to each region. Th |
| `Enum.ScaleType.Tile` | 2 | The image is tiled to fit within the element. For example, if the element is twice the X dimension o |
| `Enum.ScaleType.Fit` | 3 | The image is scaled fit within the element X or Y dimension (whichever fits first). |
| `Enum.ScaleType.Crop` | 4 | The image is cropped to fit within the element. |
