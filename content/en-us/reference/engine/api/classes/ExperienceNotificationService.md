---
title: ExperienceNotificationService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ExperienceNotificationService

Service containing methods to validate users and prompt them to enable
experience notifications.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

[Experience notifications](../../../production/promotion/experience-notifications.md)
are a way for 13+ users to keep up with their favorite experiences through
timely, personalized notifications. This service contains methods to validate
users and prompt them to enable notifications.

## Methods

### `Class.ExperienceNotificationService:CanPromptOptInAsync`

``CanPromptOptInAsync()`` -> `bool`
  [Yields]

### `Class.ExperienceNotificationService:InvokeOptInPromptClosed`

``InvokeOptInPromptClosed()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.ExperienceNotificationService:PromptOptIn`

``PromptOptIn()`` -> `null`

## Events

### `Class.ExperienceNotificationService.OptInPromptClosed`

Fires with: ()

### `Class.ExperienceNotificationService.PromptOptInRequested`

Fires with: ()
