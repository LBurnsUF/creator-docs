---
title: GeometryService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# GeometryService

Service containing geometric operations.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

Service containing geometric operations not directly related to specific
objects.

## Methods

### `Class.GeometryService:CalculateConstraintsToPreserve`

``CalculateConstraintsToPreserve(source: `Class.Instance`, destination: `Array`, options: `Dictionary`)`` -> `Array`

### `Class.GeometryService:CreateSolidPrimitive`

``CreateSolidPrimitive(type: `Enum.SolidPrimitiveType`, options: `Dictionary`)`` -> `Class.MeshPart`

### `Class.GeometryService:FragmentAsync`

``FragmentAsync(part: `Class.BasePart`, sites: `Array`, options: `Dictionary`)`` -> `Array`
  [Yields]

### `Class.GeometryService:GenerateFragmentSites`

``GenerateFragmentSites(part: `Class.BasePart`, options: `Dictionary`)`` -> `Array`

### `Class.GeometryService:HashMeshAsync`

``HashMeshAsync(meshId: `Datatype.ContentId`)`` -> `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.GeometryService:IntersectAsync`

``IntersectAsync(part: `Class.Instance`, parts: `Array`, options: `Dictionary`)`` -> `Array`
  [Yields]

### `Class.GeometryService:SubtractAsync`

``SubtractAsync(part: `Class.Instance`, parts: `Array`, options: `Dictionary`)`` -> `Array`
  [Yields]

### `Class.GeometryService:SweepPartAsync`

``SweepPartAsync(part: `Class.BasePart`, cframes: `Array`, options: `Dictionary`)`` -> `Class.MeshPart`
  [Yields]

### `Class.GeometryService:TranscodeMesh`

``TranscodeMesh(instance: `Class.Instance`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.GeometryService:TranscodeModel`

``TranscodeModel(instance: `Class.Instance`)`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.GeometryService:UnionAsync`

``UnionAsync(part: `Class.Instance`, parts: `Array`, options: `Dictionary`)`` -> `Array`
  [Yields]
