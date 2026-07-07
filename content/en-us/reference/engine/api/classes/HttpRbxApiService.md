---
title: HttpRbxApiService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# HttpRbxApiService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.HttpRbxApiService:GetAsync`

``GetAsync(apiUrlPath: `string`, priority: `Enum.ThrottlingPriority`, httpRequestType: `Enum.HttpRequestType`)`` → `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.HttpRbxApiService:GetAsyncFullUrl`

``GetAsyncFullUrl(apiUrl: `string`, priority: `Enum.ThrottlingPriority`, httpRequestType: `Enum.HttpRequestType`)`` → `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.HttpRbxApiService:GetDocumentationUrl`

``GetDocumentationUrl(partialUrl: `string`)`` → `string`
   {security: RobloxScriptSecurity}

### `Class.HttpRbxApiService:PostAsync`

``PostAsync(apiUrlPath: `string`, data: `string`, priority: `Enum.ThrottlingPriority`, content_type: `Enum.HttpContentType`, httpRequestType: `Enum.HttpRequestType`)`` → `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.HttpRbxApiService:PostAsyncFullUrl`

``PostAsyncFullUrl(apiUrl: `string`, data: `string`, priority: `Enum.ThrottlingPriority`, content_type: `Enum.HttpContentType`, httpRequestType: `Enum.HttpRequestType`)`` → `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.HttpRbxApiService:RequestAsync`

``RequestAsync(requestOptions: `Dictionary`, priority: `Enum.ThrottlingPriority`, content_type: `Enum.HttpContentType`, httpRequestType: `Enum.HttpRequestType`)`` → `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.HttpRbxApiService:RequestLimitedAsync`

``RequestLimitedAsync(requestOptions: `Dictionary`, priority: `Enum.ThrottlingPriority`, content_type: `Enum.HttpContentType`, httpRequestType: `Enum.HttpRequestType`)`` → `string`
  [Yields]
