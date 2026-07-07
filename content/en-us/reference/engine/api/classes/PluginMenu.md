---
title: PluginMenu
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# PluginMenu

**Inherits**: Instance > Object

**Tags**: NotCreatable, NotReplicated

## Properties

- **Icon**: `string` [NotReplicated]
- **Title**: `string` [NotReplicated]
- **Visible**: `bool` (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **AddAction**(`action: Instance`) -> `null`
- **AddMenu**(`menu: Instance`) -> `null`
- **AddNewAction**(`actionId: string`, `text: string`, `icon: string = `) -> `Instance`
- **AddSeparator**() -> `null`
- **Clear**() -> `null`
- **ShowAsync**() -> `Instance` [Yields]
