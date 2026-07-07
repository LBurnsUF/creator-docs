---
title: UnvalidatedAssetService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# UnvalidatedAssetService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **AppendTempAssetId**(`userId: int64`, `id: int64`, `lookAt: Vector3`, `camPos: Vector3`, `usage: string`) -> `null`
- **AppendVantagePoint**(`userId: int64`, `id: int64`, `lookAt: Vector3`, `camPos: Vector3`) -> `bool`
- **UpgradeTempAssetId**(`userId: int64`, `tempId: int64`, `assetId: int64`) -> `bool`
