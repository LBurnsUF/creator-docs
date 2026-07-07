---
title: RibbonNotificationService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# RibbonNotificationService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **OnNotificationUpdateFromPlugin**(`newNotificationId: string`, `seenNotificationId: string`) -> `null`

## Events

- **AllNotificationsReadFromRibbon**()
- **NewNotificationFromRibbon**(`newNotificationId: string`)
- **NotificationReadFromRibbon**(`newNotificationId: string`)
- **ToggleNotificationTray**(`checked: bool`, `newNotificationAvailable: bool`)
