---
title: PackageUIService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# PackageUIService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.PackageUIService:ConvertToMockPackage`

``ConvertToMockPackage(instance: `Class.Instance`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.PackageUIService:ConvertToPackageAsync`

``ConvertToPackageAsync(sourceRoot: `Class.Instance`, name: `string`, cloneRoot: `Class.Instance`)`` -> `Class.Instance`
  [Yields] {security: RobloxScriptSecurity}

### `Class.PackageUIService:ConvertToPackageClosedCallback`

``ConvertToPackageClosedCallback(sourceRoot: `Class.Instance`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.PackageUIService:ConvertToPackageUpload`

``ConvertToPackageUpload(uploadUrl: `string`, cloneInstances: `Datatype.Instances`, originalInstances: `Datatype.Instances`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.PackageUIService:GetPackageInfo`

``GetPackageInfo(packageAssetId: `int64`)`` -> `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.PackageUIService:PublishPackage`

``PublishPackage(packageInstance: `Class.Instance`, addUndoWayPoint: `bool`)`` -> `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.PackageUIService:SetPackageVersion`

``SetPackageVersion(packageInstance: `Class.Instance`, versionNumber: `int64`)`` -> `Class.Instance`
  [Yields] {security: RobloxScriptSecurity}

## Events

### `Class.PackageUIService.OnConvertToPackageResult`

Fires with: (isSuccessful: `bool`, errorMessage: `string`)

### `Class.PackageUIService.OnOpenConvertToPackagePlugin`

Fires with: (instances: `Datatype.Instances`, name: `string`, cloneInstances: `Datatype.Instances`)
