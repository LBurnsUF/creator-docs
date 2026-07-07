---
title: SessionService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# SessionService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.SessionService:AcquireContextFocus`

``AcquireContextFocus(context: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SessionService:GenerateSessionInfoString`

``GenerateSessionInfoString(includeArbitrarySessions: `bool`, includeTag: `bool`, includeTimestamps: `bool`, includeMetadata: `bool`)`` → `string`
   {security: RobloxScriptSecurity}

### `Class.SessionService:GetBreadcrumbs`

``GetBreadcrumbs()`` → `Array`
   {security: RobloxScriptSecurity}

### `Class.SessionService:GetCreatedTimestampUtcMs`

``GetCreatedTimestampUtcMs(sid: `string`)`` → `int64`
   {security: RobloxScriptSecurity}

### `Class.SessionService:GetHistory`

``GetHistory()`` → `Array`
   {security: RobloxScriptSecurity}

### `Class.SessionService:GetMetadata`

``GetMetadata(sid: `string`, key: `string`)`` → `Variant`
   {security: RobloxScriptSecurity}

### `Class.SessionService:GetRootSID`

``GetRootSID()`` → `string`
   {security: RobloxScriptSecurity}

### `Class.SessionService:GetSessionID`

``GetSessionID(structuralId: `string`)`` → `string`
   {security: RobloxScriptSecurity}

### `Class.SessionService:GetSessionTag`

``GetSessionTag(sid: `string`)`` → `string`
   {security: RobloxScriptSecurity}

### `Class.SessionService:IsContextFocused`

``IsContextFocused(context: `string`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.SessionService:ReleaseContextFocus`

``ReleaseContextFocus(context: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SessionService:RemoveMetadata`

``RemoveMetadata(sid: `string`, key: `string`, context: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SessionService:RemoveSession`

``RemoveSession(sid: `string`, context: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SessionService:RemoveSessionsWithMetadataKey`

``RemoveSessionsWithMetadataKey(key: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SessionService:ReplaceSession`

``ReplaceSession(sid: `string`, tag: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SessionService:SessionExists`

``SessionExists(sid: `string`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.SessionService:SetMetadata`

``SetMetadata(sid: `string`, key: `string`, value: `Variant`, context: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SessionService:SetSession`

``SetSession(parentSid: `string`, childSid: `string`, tag: `string`, context: `string`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.SessionService.SessionChanged`

Fires with: (structuralId: `string`, currentTag: `string`, currentSessionId: `string`, previousTag: `string`, previousSessionId: `string`)
