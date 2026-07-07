---
title: MLService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# MLService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **CreateSessionAsync**(`assetId: string`) -> `MLSession` [Yields]
- **GetNPCInferenceSpecAsync**(`server: string`, `port: int`) -> `Dictionary` [Yields]
- **IsPostProcessReady**() -> `bool`
- **LoadPostProcessModelAsync**(`assetId: int64`) -> `null` [Yields]
- **RunNPCInferenceAsync**(`server: string`, `port: int`, `features: Dictionary`) -> `Dictionary` [Yields]
- **SetPostProcessEnabled**(`enabled: bool`) -> `null`
