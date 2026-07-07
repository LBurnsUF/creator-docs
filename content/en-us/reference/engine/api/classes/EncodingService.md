---
title: EncodingService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# EncodingService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **Base64Decode**(`input: buffer`) -> `buffer`
- **Base64Encode**(`input: buffer`) -> `buffer`
- **CompressBuffer**(`input: buffer`, `algorithm: CompressionAlgorithm`, `compressionLevel: int = 1`) -> `buffer`
- **ComputeBufferHash**(`input: buffer`, `algorithm: HashAlgorithm`) -> `buffer`
- **ComputeStringHash**(`input: string`, `algorithm: HashAlgorithm`) -> `string`
- **DecompressBuffer**(`input: buffer`, `algorithm: CompressionAlgorithm`) -> `buffer`
- **GetDecompressedBufferSize**(`input: buffer`, `algorithm: CompressionAlgorithm`) -> `int?`
