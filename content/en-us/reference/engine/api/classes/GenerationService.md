---
title: GenerationService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# GenerationService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **ConnectAsync**(`sessionId: string`, `sdp: string`, `type: string`, `relay: string`) -> `Tuple` [Yields]
- **DisconnectAsync**(`sessionId: string`) -> `bool` [Yields]
- **GenerateMeshAsync**(`inputs: Dictionary`, `player: Player`, `options: Dictionary`, `intermediateResultCallback: Function?`) -> `Tuple` [Yields]
- **GenerateModelAsync**(`inputs: Dictionary`, `schema: Dictionary`, `options: Dictionary?`) -> `Tuple` [Yields]
- **GetVideoGenSessionAsync**() -> `Tuple` [Yields]
- **GetVideoGenTriggersAsync**(`sessionId: string`, `lookbackSeconds: int`) -> `Dictionary` [Yields]
- **InternalGenerateMeshAsync**(`inputs: Dictionary`, `userId: int64`, `options: Dictionary`, `intermediateResultCallback: Function?`) -> `Tuple` [Yields]
- **LoadGeneratedMeshAsync**(`generationId: string`) -> `MeshPart` [Yields]
- **LoadModelFromGlbAsync**(`glbPath: string`) -> `Model` [Yields]
- **StartVideoGenSessionAsync**(`sessionId: string`, `prompt: string`, `imageData: string`, `imageS3Reference: string`, `triggers: Dictionary`) -> `bool` [Yields]
- **UpdateVideoGenSessionPromptAsync**(`sessionId: string`, `prompt: string`, `imageData: string`, `imageS3Reference: string`, `mode: string`) -> `bool` [Yields]
- **UpdateVideoGenSessionTriggersAsync**(`sessionId: string`, `triggers: Dictionary`) -> `bool` [Yields]
