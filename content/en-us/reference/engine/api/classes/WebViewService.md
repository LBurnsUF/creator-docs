---
title: WebViewService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# WebViewService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **CloseWindow**() -> `null`
- **IsAvailable**() -> `bool` [Yields]
- **MutateWindow**(`url: string`, `title: string?`, `isVisible: bool?`, `searchType: string?`, `transitionAnimation: string?`, `showDomainAsTitle: bool?`, `backButtonVisible: bool?`) -> `null`
- **OpenWindow**(`url: string`, `title: string?`, `isVisible: bool?`, `searchType: string?`, `transitionAnimation: string?`, `showDomainAsTitle: bool?`, `backButtonVisible: bool?`) -> `null`
- **OpenWindowV2**(`url: string`, `params: WebViewParams?`) -> `null`

## Events

- **OnJavaScriptCall**(`content: string`)
- **OnWindowClosed**()
