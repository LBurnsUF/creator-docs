---
title: AssetQualityService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# AssetQualityService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **FetchAssetQualitySummaryFromGltfAsync**(`gltfData: string`, `desiredQualityChecks: Array`) -> `Dictionary` [Yields]
- **FetchAssetQualitySummaryFromJobIdAsync**(`jobId: string`, `desiredQualityChecks: Array`) -> `Dictionary` [Yields]
- **FetchAssetQualityValidationEntriesFromModelsAsync**(`models: Array`, `assetTypeIds: Array`, `settings: Dictionary`) -> `Dictionary` [Yields]
- **FetchAssetQualityVisualizationDataFromUrlAsync**(`visualizationUrl: string`) -> `Dictionary` [Yields]
- **GenerateAssetQualityGltfFromInstanceAsync**(`uploadModel: Model`) -> `string` [Yields]
