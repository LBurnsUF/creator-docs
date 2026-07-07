---
title: GeometryService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# GeometryService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **CalculateConstraintsToPreserve**(`source: Instance`, `destination: Array`, `options: Dictionary = nil`) -> `Array`
- **CreateSolidPrimitive**(`type: SolidPrimitiveType`, `options: Dictionary = nil`) -> `MeshPart`
- **FragmentAsync**(`part: BasePart`, `sites: Array`, `options: Dictionary = nil`) -> `Array` [Yields]
- **GenerateFragmentSites**(`part: BasePart`, `options: Dictionary = nil`) -> `Array`
- **HashMeshAsync**(`meshId: ContentId`) -> `string` [Yields]
- **IntersectAsync**(`part: Instance`, `parts: Array`, `options: Dictionary = nil`) -> `Array` [Yields]
- **SubtractAsync**(`part: Instance`, `parts: Array`, `options: Dictionary = nil`) -> `Array` [Yields]
- **SweepPartAsync**(`part: BasePart`, `cframes: Array`, `options: Dictionary = nil`) -> `MeshPart` [Yields]
- **TranscodeMesh**(`instance: Instance`) -> `null`
- **TranscodeModel**(`instance: Instance`) -> `Array`
- **UnionAsync**(`part: Instance`, `parts: Array`, `options: Dictionary = nil`) -> `Array` [Yields]
