---
title: AssetQualityService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# AssetQualityService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.AssetQualityService:FetchAssetQualitySummaryFromGltfAsync`

``FetchAssetQualitySummaryFromGltfAsync(gltfData: `string`, desiredQualityChecks: `Array`)`` → `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AssetQualityService:FetchAssetQualitySummaryFromJobIdAsync`

``FetchAssetQualitySummaryFromJobIdAsync(jobId: `string`, desiredQualityChecks: `Array`)`` → `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AssetQualityService:FetchAssetQualityValidationEntriesFromModelsAsync`

``FetchAssetQualityValidationEntriesFromModelsAsync(models: `Array`, assetTypeIds: `Array`, settings: `Dictionary`)`` → `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AssetQualityService:FetchAssetQualityVisualizationDataFromUrlAsync`

``FetchAssetQualityVisualizationDataFromUrlAsync(visualizationUrl: `string`)`` → `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AssetQualityService:GenerateAssetQualityGltfFromInstanceAsync`

``GenerateAssetQualityGltfFromInstanceAsync(uploadModel: `Class.Model`)`` → `string`
  [Yields] {security: RobloxScriptSecurity}
