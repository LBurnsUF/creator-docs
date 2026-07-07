---
title: IXPService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# IXPService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **ClearCreatorLayers**() -> `null`
- **ClearUserLayers**() -> `null`
- **GetBrowserTrackerLayerLoadingStatus**() -> `IXPLoadingStatus`
- **GetBrowserTrackerLayerVariables**(`layerName: string`) -> `Dictionary`
- **GetBrowserTrackerStatusForLayer**(`layerName: string`) -> `IXPLoadingStatus?`
- **GetCreatorLayerLoadingStatus**() -> `IXPLoadingStatus`
- **GetCreatorLayerVariables**(`layerName: string`) -> `Dictionary`
- **GetCreatorStatusForLayer**(`layerName: string`) -> `IXPLoadingStatus?`
- **GetRegisteredCreatorLayersToStatus**() -> `Dictionary`
- **GetRegisteredUserLayersToStatus**() -> `Dictionary`
- **GetUserLayerLoadingStatus**() -> `IXPLoadingStatus`
- **GetUserLayerVariables**(`layerName: string`) -> `Dictionary`
- **GetUserStatusForLayer**(`layerName: string`) -> `IXPLoadingStatus?`
- **InitializeCreatorLayers**(`creatorId: int64`) -> `null`
- **InitializeUserLayers**(`userId: int64`) -> `null`
- **LogBrowserTrackerLayerExposure**(`layerName: string`) -> `null`
- **LogCreatorLayerExposure**(`layerName: string`) -> `null`
- **LogFlagLinkedUserLayerExposure**(`layerName: string`) -> `null`
- **LogUserLayerExposure**(`layerName: string`) -> `null`
- **RegisterCreatorLayers**(`creatorLayers: Variant`) -> `null`
- **RegisterUserLayers**(`userLayers: Variant`) -> `null`

## Events

- **OnBrowserTrackerLayerLoadingStatusChanged**(`status: IXPLoadingStatus`)
- **OnCreatorLayerLoadingStatusChanged**(`status: IXPLoadingStatus`)
- **OnUserLayerLoadingStatusChanged**(`status: IXPLoadingStatus`)
