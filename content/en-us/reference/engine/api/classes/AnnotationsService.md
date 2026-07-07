---
title: AnnotationsService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# AnnotationsService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.AnnotationsService.AnnotationsLoadingStatus` | `Enum.AnnotationRequestStatus` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.AnnotationsService.AnnotationsVisible` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.AnnotationsService.Hovered` | `Class.Annotation` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.AnnotationsService.Mode` | `Enum.AnnotationEditingMode` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.AnnotationsService.ResolvedLoadingStatus` | `Enum.AnnotationRequestStatus` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.AnnotationsService.Selected` | `Class.Annotation` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |

## Methods

### `Class.AnnotationsService:CreateAnnotation`

``CreateAnnotation(annotation: `Class.Annotation`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AnnotationsService:CreateOrUpdateChannelPreferenceAsync`

``CreateOrUpdateChannelPreferenceAsync(userId: `int64`, channelId: `string`, placeId: `int64`, channelContentPreference: `Enum.AnnotationChannelContentPreference`)`` → `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AnnotationsService:CreateOrUpdatePlacePreference`

``CreateOrUpdatePlacePreference(placeId: `int64`, userId: `int64`, placeContentPreference: `Enum.PlaceContentPreference`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AnnotationsService:CreateOrUpdatePlacePreferenceAsync`

``CreateOrUpdatePlacePreferenceAsync(userId: `int64`, placeContentPreference: `Enum.AnnotationPlaceContentPreference`, placeId: `int64`)`` → `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AnnotationsService:DeleteAnnotation`

``DeleteAnnotation(annotation: `Class.Annotation`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AnnotationsService:EditAnnotation`

``EditAnnotation(uniqueId: `string`, contents: `string`, taggedUsers: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AnnotationsService:GetAnnotationThreads`

``GetAnnotationThreads()`` → `Datatype.Instances`
   {security: RobloxScriptSecurity}

### `Class.AnnotationsService:GetChannelPreferenceAsync`

``GetChannelPreferenceAsync(userId: `int64`, channelId: `string`, placeId: `int64`)`` → `Enum.AnnotationChannelContentPreference`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AnnotationsService:GetPlacePreference`

``GetPlacePreference(placeId: `int64`, userId: `int64`)`` → `Enum.PlaceContentPreference`
   {security: RobloxScriptSecurity}

### `Class.AnnotationsService:GetPlacePreferenceAsync`

``GetPlacePreferenceAsync(userId: `int64`, placeId: `int64`)`` → `Enum.AnnotationPlaceContentPreference`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AnnotationsService:LoadAnnotationReplies`

``LoadAnnotationReplies(annotation: `Class.Annotation`, reverseOrder: `bool`, loadAll: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AnnotationsService:LoadAnnotations`

``LoadAnnotations(resolved: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AnnotationsService:LoadResolvedAnnotations`

``LoadResolvedAnnotations(count: `int`)`` → `null`
  [Deprecated] {security: RobloxScriptSecurity}

### `Class.AnnotationsService:ResolveAnnotation`

``ResolveAnnotation(annotation: `Class.Annotation`, resolved: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.AnnotationsService.AnnotationAdded`

Fires with: (requestId: `string`, annotation: `Class.Annotation`, channelId: `string`)

### `Class.AnnotationsService.AnnotationDeleted`

Fires with: (requestId: `string`, annotation: `Class.Annotation`)

### `Class.AnnotationsService.AnnotationEdited`

Fires with: (requestId: `string`, uniqueId: `string`, contents: `string`, taggedUsers: `string`)

### `Class.AnnotationsService.AnnotationResolved`

Fires with: (requestId: `string`, annotation: `Class.Annotation`, resolved: `bool`)

### `Class.AnnotationsService.ServerLoadAnnotationReplies`

Fires with: (annotation: `Class.Annotation`, reverseOrder: `bool`, loadAll: `bool`)

### `Class.AnnotationsService.ServerLoadAnnotations`

Fires with: (resolved: `bool`)

### `Class.AnnotationsService.ServerLoadResolvedAnnotations`

Fires with: (count: `int`)
