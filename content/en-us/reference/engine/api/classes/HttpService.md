---
title: HttpService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# HttpService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **HttpEnabled**: `bool` (Security: Read=None, Write=LocalUserSecurity)

## Methods

- **CreateWebStreamClient**(`streamClientType: WebStreamClientType`, `requestOptions: Dictionary`) -> `WebStreamClient`
- **CreateWebStreamClientInternal**(`streamClientType: WebStreamClientType`, `requestOptions: Dictionary`) -> `WebStreamClient`
- **GenerateGUID**(`wrapInCurlyBraces: bool = true`) -> `string`
- **GetAsync**(`url: Variant`, `nocache: bool = false`, `headers: Variant`) -> `string` [Yields]
- **GetHttpEnabled**() -> `bool`
- **GetSecret**(`key: string`) -> `Secret`
- **GetUserAgent**() -> `string`
- **JSONDecode**(`input: string`) -> `Variant` [CustomLuaState]
- **JSONDecodeAsync**(`input: string`) -> `Variant` [Yields]
- **JSONEncode**(`input: Variant`) -> `string` [CustomLuaState]
- **JSONEncodeAsync**(`obj: Variant`) -> `string` [Yields]
- **PostAsync**(`url: Variant`, `data: string`, `content_type: HttpContentType = ApplicationJson`, `compress: bool = false`, `headers: Variant`) -> `string` [Yields]
- **RequestAccessTokenScopesAsync**(`requiredScopes: Array`) -> `Secret` [Yields]
- **RequestAsync**(`requestOptions: Dictionary`) -> `Dictionary` [Yields]
- **RequestInternal**(`options: Dictionary`) -> `Instance`
- **SetHttpEnabled**(`enabled: bool`) -> `null`
- **UrlEncode**(`input: string`) -> `string`
