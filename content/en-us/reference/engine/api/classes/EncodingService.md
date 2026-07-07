---
title: EncodingService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# EncodingService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.EncodingService:Base64Decode`

``Base64Decode(input: `Datatype.buffer`)`` → `Datatype.buffer`

### `Class.EncodingService:Base64Encode`

``Base64Encode(input: `Datatype.buffer`)`` → `Datatype.buffer`

### `Class.EncodingService:CompressBuffer`

``CompressBuffer(input: `Datatype.buffer`, algorithm: `Enum.CompressionAlgorithm`, compressionLevel: `int`)`` → `Datatype.buffer`

### `Class.EncodingService:ComputeBufferHash`

``ComputeBufferHash(input: `Datatype.buffer`, algorithm: `Enum.HashAlgorithm`)`` → `Datatype.buffer`

### `Class.EncodingService:ComputeStringHash`

``ComputeStringHash(input: `string`, algorithm: `Enum.HashAlgorithm`)`` → `string`

### `Class.EncodingService:DecompressBuffer`

``DecompressBuffer(input: `Datatype.buffer`, algorithm: `Enum.CompressionAlgorithm`)`` → `Datatype.buffer`

### `Class.EncodingService:GetDecompressedBufferSize`

``GetDecompressedBufferSize(input: `Datatype.buffer`, algorithm: `Enum.CompressionAlgorithm`)`` → `int?`
