---
title: HttpRbxApiService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# HttpRbxApiService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **GetAsync**(`apiUrlPath: string`, `priority: ThrottlingPriority = Default`, `httpRequestType: HttpRequestType = Default`) -> `string` [Yields]
- **GetAsyncFullUrl**(`apiUrl: string`, `priority: ThrottlingPriority = Default`, `httpRequestType: HttpRequestType = Default`) -> `string` [Yields]
- **GetDocumentationUrl**(`partialUrl: string`) -> `string`
- **PostAsync**(`apiUrlPath: string`, `data: string`, `priority: ThrottlingPriority = Default`, `content_type: HttpContentType = ApplicationJson`, `httpRequestType: HttpRequestType = Default`) -> `string` [Yields]
- **PostAsyncFullUrl**(`apiUrl: string`, `data: string`, `priority: ThrottlingPriority = Default`, `content_type: HttpContentType = ApplicationJson`, `httpRequestType: HttpRequestType = Default`) -> `string` [Yields]
- **RequestAsync**(`requestOptions: Dictionary`, `priority: ThrottlingPriority = Default`, `content_type: HttpContentType = ApplicationJson`, `httpRequestType: HttpRequestType = Default`) -> `string` [Yields]
- **RequestLimitedAsync**(`requestOptions: Dictionary`, `priority: ThrottlingPriority = Default`, `content_type: HttpContentType = ApplicationJson`, `httpRequestType: HttpRequestType = Default`) -> `string` [Yields]
