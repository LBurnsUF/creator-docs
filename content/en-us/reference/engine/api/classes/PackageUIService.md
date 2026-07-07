---
title: PackageUIService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# PackageUIService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **ConvertToMockPackage**(`instance: Instance`) -> `null`
- **ConvertToPackageAsync**(`sourceRoot: Instance`, `name: string`, `cloneRoot: Instance`) -> `Instance` [Yields]
- **ConvertToPackageClosedCallback**(`sourceRoot: Instance`) -> `null`
- **ConvertToPackageUpload**(`uploadUrl: string`, `cloneInstances: Instances`, `originalInstances: Instances`) -> `null`
- **GetPackageInfo**(`packageAssetId: int64`) -> `Dictionary` [Yields]
- **PublishPackage**(`packageInstance: Instance`, `addUndoWayPoint: bool`) -> `null` [Yields]
- **SetPackageVersion**(`packageInstance: Instance`, `versionNumber: int64`) -> `Instance` [Yields]

## Events

- **OnConvertToPackageResult**(`isSuccessful: bool`, `errorMessage: string`)
- **OnOpenConvertToPackagePlugin**(`instances: Instances`, `name: string`, `cloneInstances: Instances`)
