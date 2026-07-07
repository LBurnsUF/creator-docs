---
title: WebViewService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# WebViewService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.WebViewService:CloseWindow`

``CloseWindow()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.WebViewService:IsAvailable`

``IsAvailable()`` → `bool`
  [Yields] {security: RobloxScriptSecurity}

### `Class.WebViewService:MutateWindow`

``MutateWindow(url: `string`, title: `string?`, isVisible: `bool?`, searchType: `string?`, transitionAnimation: `string?`, showDomainAsTitle: `bool?`, backButtonVisible: `bool?`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.WebViewService:OpenWindow`

``OpenWindow(url: `string`, title: `string?`, isVisible: `bool?`, searchType: `string?`, transitionAnimation: `string?`, showDomainAsTitle: `bool?`, backButtonVisible: `bool?`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.WebViewService:OpenWindowV2`

``OpenWindowV2(url: `string`, params: `Datatype.WebViewParams`?)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.WebViewService.OnJavaScriptCall`

Fires with: (content: `string`)

### `Class.WebViewService.OnWindowClosed`

Fires with: ()
