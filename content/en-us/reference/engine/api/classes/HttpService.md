---
title: HttpService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# HttpService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.HttpService.HttpEnabled` | `bool` |  {write: LocalUserSecurity} |

## Methods

### `Class.HttpService:CreateWebStreamClient`

``CreateWebStreamClient(streamClientType: `Enum.WebStreamClientType`, requestOptions: `Dictionary`)`` → `Class.WebStreamClient`

### `Class.HttpService:CreateWebStreamClientInternal`

``CreateWebStreamClientInternal(streamClientType: `Enum.WebStreamClientType`, requestOptions: `Dictionary`)`` → `Class.WebStreamClient`
   {security: RobloxScriptSecurity}

### `Class.HttpService:GenerateGUID`

``GenerateGUID(wrapInCurlyBraces: `bool`)`` → `string`

### `Class.HttpService:GetAsync`

``GetAsync(url: `Variant`, nocache: `bool`, headers: `Variant`)`` → `string`
  [Yields]

### `Class.HttpService:GetHttpEnabled`

``GetHttpEnabled()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.HttpService:GetSecret`

``GetSecret(key: `string`)`` → `Datatype.Secret`

### `Class.HttpService:GetUserAgent`

``GetUserAgent()`` → `string`
   {security: RobloxScriptSecurity}

### `Class.HttpService:JSONDecode`

``JSONDecode(input: `string`)`` → `Variant`
  [CustomLuaState]

### `Class.HttpService:JSONDecodeAsync`

``JSONDecodeAsync(input: `string`)`` → `Variant`
  [Yields] {security: RobloxScriptSecurity}

### `Class.HttpService:JSONEncode`

``JSONEncode(input: `Variant`)`` → `string`
  [CustomLuaState]

### `Class.HttpService:JSONEncodeAsync`

``JSONEncodeAsync(obj: `Variant`)`` → `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.HttpService:PostAsync`

``PostAsync(url: `Variant`, data: `string`, content_type: `Enum.HttpContentType`, compress: `bool`, headers: `Variant`)`` → `string`
  [Yields]

### `Class.HttpService:RequestAccessTokenScopesAsync`

``RequestAccessTokenScopesAsync(requiredScopes: `Array`)`` → `Datatype.Secret`
  [Yields] {security: LocalUserSecurity}

### `Class.HttpService:RequestAsync`

``RequestAsync(requestOptions: `Dictionary`)`` → `Dictionary`
  [Yields]

### `Class.HttpService:RequestInternal`

``RequestInternal(options: `Dictionary`)`` → `Class.Instance`
   {security: RobloxScriptSecurity}

### `Class.HttpService:SetHttpEnabled`

``SetHttpEnabled(enabled: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.HttpService:UrlEncode`

``UrlEncode(input: `string`)`` → `string`
