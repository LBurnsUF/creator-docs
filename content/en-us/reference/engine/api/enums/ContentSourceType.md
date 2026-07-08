---
title: ContentSourceType
type: enum
---

# `Enum.ContentSourceType`

The source type of a `Datatype.Content` value.

The source type of `Datatype.Content` value. Indicates which properties of a
`Datatype.Content` contain the referenced content.

The `Enum.ContentSourceType` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ContentSourceType.None` | 0 | Empty value with no source type. Does not reference any content or hold any non‑`nil` value. |
| `Enum.ContentSourceType.Uri` | 1 | An [asset URI](../../../projects/assets/index.md#asset-uris) `string` value contained in `Datatype.C |
| `Enum.ContentSourceType.Object` | 2 | A non-`nil` `Class.Object` reference contained in `Datatype.Content.Object`. |
| `Enum.ContentSourceType.Opaque` | 3 | A non-`nil` `Opaque` reference contained in `Datatype.Content.Opaque`. |
