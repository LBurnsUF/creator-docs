---
title: CatalogSearchParams
type: datatype
---

# `Datatype.CatalogSearchParams`

Stores parameters used in catalog searches via
`Class.AvatarEditorService:SearchCatalogAsync()`.

## Description

The `Datatype.CatalogSearchParams` data type stores the parameters of a
catalog search via `Class.AvatarEditorService:SearchCatalogAsync()`.

When accessing the value of the `Datatype.CatalogSearchParams.BundleTypes` or
`Datatype.CatalogSearchParams.AssetTypes` property the returned table will be
read-only to avoid confusion when not directly accessing the
`Datatype.CatalogSearchParams` instance.

For example, you can use these properties as follows:

```lua
local params = CatalogSearchParams.new()
params.SearchKeyword = "Test"
params.MinPrice = 5000
params.MaxPrice = 10000
params.BundleTypes = {Enum.BundleType.Animations, Enum.BundleType.BodyParts}

local types = params.BundleTypes
for _, val in types do
  print(val)
end
-- table.insert(types, Enum.BundleType.Animations) -- This would not work because the table is read only
```

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `CatalogSearchParams.SearchKeyword` | `string` | The keyword to search for catalog results with. |
| `CatalogSearchParams.MinPrice` | `number` | The minimum item price to search for. |
| `CatalogSearchParams.MaxPrice` | `number` | The maximum item price to search for. |
| `CatalogSearchParams.SortType` | `CatalogSortType` | The order in which to sort the results. |
| `CatalogSearchParams.SortAggregation` | `Enum.CatalogSortAggregation` | The time period to use to aggregate the sort results. |
| `CatalogSearchParams.CategoryFilter` | `CatalogCategoryFilter` | The category to filter the search by. |
| `CatalogSearchParams.SalesTypeFilter` | `Enum.SalesTypeFilter` | The sales type filter the search by. |
| `CatalogSearchParams.BundleTypes` | `Array<BundleType>` | An array containing `Enum.BundleType` values to filter the search by. |
| `CatalogSearchParams.AssetTypes` | `Array<AvatarAssetType>` | An array containing `Enum.AvatarAssetType` values to filter the search by. |
| `CatalogSearchParams.IncludeOffSale` | `bool` | Whether off sale items should be included in the results. |
| `CatalogSearchParams.CreatorName` | `string` | Search for items with the given creator name. |
| `CatalogSearchParams.CreatorType` | `Enum.CreatorTypeFilter` | Search for items created by the given creator type. |
| `CatalogSearchParams.CreatorId` | `number` | Search for items created by the given creator ID. |
| `CatalogSearchParams.Limit` | `number` | Specifies the number of items to return. Accepts `10`, `28`, `30`, `60`, and `120`. Defaults to `30` |

## API Usage (2 locations)

### Used as Parameter Type

- `Class.AvatarEditorService:SearchCatalog` (parameter `searchParameters`)
- `Class.AvatarEditorService:SearchCatalogAsync` (parameter `searchParameters`)
