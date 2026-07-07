---
title: AnnotationsService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# AnnotationsService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **AnnotationsLoadingStatus**: `AnnotationRequestStatus` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **AnnotationsVisible**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Hovered**: `Annotation` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Mode**: `AnnotationEditingMode` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **ResolvedLoadingStatus**: `AnnotationRequestStatus` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Selected**: `Annotation` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **CreateAnnotation**(`annotation: Annotation`) -> `null`
- **CreateOrUpdateChannelPreferenceAsync**(`userId: int64`, `channelId: string`, `placeId: int64`, `channelContentPreference: AnnotationChannelContentPreference`) -> `null` [Yields]
- **CreateOrUpdatePlacePreference**(`placeId: int64`, `userId: int64`, `placeContentPreference: PlaceContentPreference`) -> `null`
- **CreateOrUpdatePlacePreferenceAsync**(`userId: int64`, `placeContentPreference: AnnotationPlaceContentPreference`, `placeId: int64`) -> `null` [Yields]
- **DeleteAnnotation**(`annotation: Annotation`) -> `null`
- **EditAnnotation**(`uniqueId: string`, `contents: string`, `taggedUsers: string`) -> `null`
- **GetAnnotationThreads**() -> `Instances`
- **GetChannelPreferenceAsync**(`userId: int64`, `channelId: string`, `placeId: int64`) -> `AnnotationChannelContentPreference` [Yields]
- **GetPlacePreference**(`placeId: int64`, `userId: int64`) -> `PlaceContentPreference`
- **GetPlacePreferenceAsync**(`userId: int64`, `placeId: int64`) -> `AnnotationPlaceContentPreference` [Yields]
- **LoadAnnotationReplies**(`annotation: Annotation`, `reverseOrder: bool`, `loadAll: bool`) -> `null`
- **LoadAnnotations**(`resolved: bool`) -> `null`
- **LoadResolvedAnnotations**(`count: int`) -> `null` [Deprecated]
- **ResolveAnnotation**(`annotation: Annotation`, `resolved: bool`) -> `null`

## Events

- **AnnotationAdded**(`requestId: string`, `annotation: Annotation`, `channelId: string`)
- **AnnotationDeleted**(`requestId: string`, `annotation: Annotation`)
- **AnnotationEdited**(`requestId: string`, `uniqueId: string`, `contents: string`, `taggedUsers: string`)
- **AnnotationResolved**(`requestId: string`, `annotation: Annotation`, `resolved: bool`)
- **ServerLoadAnnotationReplies**(`annotation: Annotation`, `reverseOrder: bool`, `loadAll: bool`)
- **ServerLoadAnnotations**(`resolved: bool`)
- **ServerLoadResolvedAnnotations**(`count: int`)
