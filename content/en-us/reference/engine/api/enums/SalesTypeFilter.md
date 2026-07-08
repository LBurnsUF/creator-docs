---
title: SalesTypeFilter
type: enum
---

# `Enum.SalesTypeFilter`

Filters catalog search results by sales type.

The `Enum.SalesTypeFilter` enum is used with
`Datatype.CatalogSearchParams.SalesTypeFilter` to filter catalog search
results by their sales type when calling
`Class.AvatarEditorService:SearchCatalogAsync()`.

The `Enum.SalesTypeFilter` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.SalesTypeFilter.All` | 1 | Returns all items regardless of sales type. |
| `Enum.SalesTypeFilter.Collectibles` | 2 | Returns only collectible items (Limited and Limited Unique). |
| `Enum.SalesTypeFilter.Premium` | 3 | Returns only items with Premium pricing. |
| `Enum.SalesTypeFilter.TimedOptions` | 4 | Returns only items that have timed options available. |
