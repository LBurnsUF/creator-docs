---
title: Annotation
type: class
superclass: Instance
---

# Annotation

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.Annotation.AuthorColor3` | `Datatype.Color3` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.Annotation.AuthorId` | `int64` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.Annotation.ChannelId` | `string` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.Annotation.Contents` | `string` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.Annotation.CreationTimeUnix` | `int64` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.Annotation.LastModifiedTimeUnix` | `int64` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.Annotation.LoadingReplies` | `bool` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.Annotation.ReplyCount` | `int64` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.Annotation.Resolved` | `bool` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.Annotation.TaggedUsers` | `string` | [Hidden] {security: RobloxScriptSecurity} |

## Methods

### `Class.Annotation:GetRequests`

``GetRequests()`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.Annotation:GetStringUniqueId`

``GetStringUniqueId()`` → `string`
   {security: RobloxScriptSecurity}

### `Class.Annotation:IsThreadParent`

``IsThreadParent()`` → `bool`
   {security: RobloxScriptSecurity}

## Events

### `Class.Annotation.RequestCompleted`

Fires with: (requestId: `string`, requestType: `Enum.AnnotationRequestType`, result: `Enum.AnnotationRequestStatus`)

### `Class.Annotation.RequestInitiated`

Fires with: (requestId: `string`, requestType: `Enum.AnnotationRequestType`)
