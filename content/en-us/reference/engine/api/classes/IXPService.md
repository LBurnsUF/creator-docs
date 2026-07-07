---
title: IXPService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# IXPService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.IXPService:ClearCreatorLayers`

``ClearCreatorLayers()`` → `null`
   {security: LocalUserSecurity}

### `Class.IXPService:ClearUserLayers`

``ClearUserLayers()`` → `null`
   {security: LocalUserSecurity}

### `Class.IXPService:GetBrowserTrackerLayerLoadingStatus`

``GetBrowserTrackerLayerLoadingStatus()`` → `Enum.IXPLoadingStatus`
   {security: LocalUserSecurity}

### `Class.IXPService:GetBrowserTrackerLayerVariables`

``GetBrowserTrackerLayerVariables(layerName: `string`)`` → `Dictionary`
   {security: LocalUserSecurity}

### `Class.IXPService:GetBrowserTrackerStatusForLayer`

``GetBrowserTrackerStatusForLayer(layerName: `string`)`` → `Enum.IXPLoadingStatus?`
   {security: LocalUserSecurity}

### `Class.IXPService:GetCreatorLayerLoadingStatus`

``GetCreatorLayerLoadingStatus()`` → `Enum.IXPLoadingStatus`
   {security: LocalUserSecurity}

### `Class.IXPService:GetCreatorLayerVariables`

``GetCreatorLayerVariables(layerName: `string`)`` → `Dictionary`
   {security: LocalUserSecurity}

### `Class.IXPService:GetCreatorStatusForLayer`

``GetCreatorStatusForLayer(layerName: `string`)`` → `Enum.IXPLoadingStatus?`
   {security: LocalUserSecurity}

### `Class.IXPService:GetRegisteredCreatorLayersToStatus`

``GetRegisteredCreatorLayersToStatus()`` → `Dictionary`
   {security: LocalUserSecurity}

### `Class.IXPService:GetRegisteredUserLayersToStatus`

``GetRegisteredUserLayersToStatus()`` → `Dictionary`
   {security: LocalUserSecurity}

### `Class.IXPService:GetUserLayerLoadingStatus`

``GetUserLayerLoadingStatus()`` → `Enum.IXPLoadingStatus`
   {security: LocalUserSecurity}

### `Class.IXPService:GetUserLayerVariables`

``GetUserLayerVariables(layerName: `string`)`` → `Dictionary`
   {security: LocalUserSecurity}

### `Class.IXPService:GetUserStatusForLayer`

``GetUserStatusForLayer(layerName: `string`)`` → `Enum.IXPLoadingStatus?`
   {security: LocalUserSecurity}

### `Class.IXPService:InitializeCreatorLayers`

``InitializeCreatorLayers(creatorId: `int64`)`` → `null`
   {security: LocalUserSecurity}

### `Class.IXPService:InitializeUserLayers`

``InitializeUserLayers(userId: `int64`)`` → `null`
   {security: LocalUserSecurity}

### `Class.IXPService:LogBrowserTrackerLayerExposure`

``LogBrowserTrackerLayerExposure(layerName: `string`)`` → `null`
   {security: LocalUserSecurity}

### `Class.IXPService:LogCreatorLayerExposure`

``LogCreatorLayerExposure(layerName: `string`)`` → `null`
   {security: LocalUserSecurity}

### `Class.IXPService:LogFlagLinkedUserLayerExposure`

``LogFlagLinkedUserLayerExposure(layerName: `string`)`` → `null`
   {security: LocalUserSecurity}

### `Class.IXPService:LogUserLayerExposure`

``LogUserLayerExposure(layerName: `string`)`` → `null`
   {security: LocalUserSecurity}

### `Class.IXPService:RegisterCreatorLayers`

``RegisterCreatorLayers(creatorLayers: `Variant`)`` → `null`
   {security: LocalUserSecurity}

### `Class.IXPService:RegisterUserLayers`

``RegisterUserLayers(userLayers: `Variant`)`` → `null`
   {security: LocalUserSecurity}

## Events

### `Class.IXPService.OnBrowserTrackerLayerLoadingStatusChanged`

Fires with: (status: `Enum.IXPLoadingStatus`)

### `Class.IXPService.OnCreatorLayerLoadingStatusChanged`

Fires with: (status: `Enum.IXPLoadingStatus`)

### `Class.IXPService.OnUserLayerLoadingStatusChanged`

Fires with: (status: `Enum.IXPLoadingStatus`)
