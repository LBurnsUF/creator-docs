---
title: SessionService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# SessionService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **AcquireContextFocus**(`context: string`) -> `null`
- **GenerateSessionInfoString**(`includeArbitrarySessions: bool`, `includeTag: bool`, `includeTimestamps: bool`, `includeMetadata: bool`) -> `string`
- **GetBreadcrumbs**() -> `Array`
- **GetCreatedTimestampUtcMs**(`sid: string`) -> `int64`
- **GetHistory**() -> `Array`
- **GetMetadata**(`sid: string`, `key: string`) -> `Variant`
- **GetRootSID**() -> `string`
- **GetSessionID**(`structuralId: string`) -> `string`
- **GetSessionTag**(`sid: string`) -> `string`
- **IsContextFocused**(`context: string`) -> `bool`
- **ReleaseContextFocus**(`context: string`) -> `null`
- **RemoveMetadata**(`sid: string`, `key: string`, `context: string = `) -> `null`
- **RemoveSession**(`sid: string`, `context: string = `) -> `null`
- **RemoveSessionsWithMetadataKey**(`key: string`) -> `null`
- **ReplaceSession**(`sid: string`, `tag: string`) -> `null`
- **SessionExists**(`sid: string`) -> `bool`
- **SetMetadata**(`sid: string`, `key: string`, `value: Variant`, `context: string = `) -> `null`
- **SetSession**(`parentSid: string`, `childSid: string`, `tag: string`, `context: string = `) -> `null`

## Events

- **SessionChanged**(`structuralId: string`, `currentTag: string`, `currentSessionId: string`, `previousTag: string`, `previousSessionId: string`)
