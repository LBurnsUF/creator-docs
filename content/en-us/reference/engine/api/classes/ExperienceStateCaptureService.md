---
title: ExperienceStateCaptureService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ExperienceStateCaptureService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **HiddenSelectionEnabled**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **IsInBackground**: `bool` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **IsInCaptureMode**: `bool` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **SelectionMode**: `ExperienceStateCaptureSelectionMode` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **CanEnterCaptureMode**() -> `bool`
- **ResetHighlight**() -> `null`
- **ToggleCaptureMode**() -> `null`

## Events

- **ItemSelectedInCaptureMode**(`instance: Instance`)
