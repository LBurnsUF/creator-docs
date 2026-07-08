---
title: HttpService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# HttpService

Allows sending HTTP requests and provides various web-related and JSON
methods.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

`HttpService` allows HTTP requests to be sent from experience servers using
`Class.HttpService:RequestAsync()|RequestAsync`,
`Class.HttpService:GetAsync()|GetAsync` and
`Class.HttpService:PostAsync()|PostAsync`. This service allows experiences to
be integrated with third-party web services such as analytics, data storage,
remote server configuration, error reporting, advanced calculations, or
real-time communication. Additionally, it can call a subset of the Open Cloud
APIs.

For more information about these use cases, see
[In-experience HTTP requests](../../../cloud-services/http-service.md).

`HttpService` also houses the `Class.HttpService:JSONEncode()|JSONEncode` and
`Class.HttpService:JSONDecode()|JSONDecode` methods, which are useful for
communicating with services that use the [JSON](https://json.org) format. In
addition, the `Class.HttpService:GenerateGUID()|GenerateGUID` method provides
random 128‑bit labels which can be treated as probabilistically unique in a
variety of scenarios.

Within Studio, use
`Class.HttpService:CreateWebStreamClient()|CreateWebStreamClient()` to process
data in real time from servers that support streaming protocols such as
[SSE](https://en.wikipedia.org/wiki/Server-sent_events),
[chunked transfer encoding](https://en.wikipedia.org/wiki/Chunked_transfer_encoding),
and [WebSockets](https://en.wikipedia.org/wiki/WebSocket). You can connect
callback functions to stream events, allowing you to process data immediately
as it arrives instead of waiting for the entire response to complete.

Only send HTTP requests to trusted third-party platforms to avoid introducing
unnecessary security risks to your experience.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.HttpService.HttpEnabled` | `bool` |  {write: LocalUserSecurity} |

## Methods

### `Class.HttpService:CreateWebStreamClient`

``CreateWebStreamClient(streamClientType: `Enum.WebStreamClientType`, requestOptions: `Dictionary`)`` -> `Class.WebStreamClient`

### `Class.HttpService:CreateWebStreamClientInternal`

``CreateWebStreamClientInternal(streamClientType: `Enum.WebStreamClientType`, requestOptions: `Dictionary`)`` -> `Class.WebStreamClient`
   {security: RobloxScriptSecurity}

### `Class.HttpService:GenerateGUID`

``GenerateGUID(wrapInCurlyBraces: `bool`)`` -> `string`

### `Class.HttpService:GetAsync`

``GetAsync(url: `Variant`, nocache: `bool`, headers: `Variant`)`` -> `string`
  [Yields]

### `Class.HttpService:GetHttpEnabled`

``GetHttpEnabled()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.HttpService:GetSecret`

``GetSecret(key: `string`)`` -> `Datatype.Secret`

### `Class.HttpService:GetUserAgent`

``GetUserAgent()`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.HttpService:JSONDecode`

``JSONDecode(input: `string`)`` -> `Variant`
  [CustomLuaState]

### `Class.HttpService:JSONDecodeAsync`

``JSONDecodeAsync(input: `string`)`` -> `Variant`
  [Yields] {security: RobloxScriptSecurity}

### `Class.HttpService:JSONEncode`

``JSONEncode(input: `Variant`)`` -> `string`
  [CustomLuaState]

### `Class.HttpService:JSONEncodeAsync`

``JSONEncodeAsync(obj: `Variant`)`` -> `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.HttpService:PostAsync`

``PostAsync(url: `Variant`, data: `string`, content_type: `Enum.HttpContentType`, compress: `bool`, headers: `Variant`)`` -> `string`
  [Yields]

### `Class.HttpService:RequestAccessTokenScopesAsync`

``RequestAccessTokenScopesAsync(requiredScopes: `Array`)`` -> `Datatype.Secret`
  [Yields] {security: LocalUserSecurity}

### `Class.HttpService:RequestAsync`

``RequestAsync(requestOptions: `Dictionary`)`` -> `Dictionary`
  [Yields]

### `Class.HttpService:RequestInternal`

``RequestInternal(options: `Dictionary`)`` -> `Class.Instance`
   {security: RobloxScriptSecurity}

### `Class.HttpService:SetHttpEnabled`

``SetHttpEnabled(enabled: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.HttpService:UrlEncode`

``UrlEncode(input: `string`)`` -> `string`
