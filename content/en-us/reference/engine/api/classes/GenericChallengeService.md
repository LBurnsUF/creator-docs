---
title: GenericChallengeService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# GenericChallengeService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.GenericChallengeService:SignalChallengeAbandoned`

``SignalChallengeAbandoned(challengeID: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.GenericChallengeService:SignalChallengeCompleted`

``SignalChallengeCompleted(challengeID: `string`, challengeType: `string`, challengeMetadata: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.GenericChallengeService:SignalChallengeInvalidated`

``SignalChallengeInvalidated(challengeID: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.GenericChallengeService:SignalChallengeLoaded`

``SignalChallengeLoaded(challengeID: `string`, success: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.GenericChallengeService:SignalChallengeRequired`

``SignalChallengeRequired(challengeID: `string`, challengeType: `string`, challengeMetadata: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.GenericChallengeService.ChallengeAbandonedEvent`

Fires with: (challengeID: `string`)

### `Class.GenericChallengeService.ChallengeCompletedEvent`

Fires with: (challengeID: `string`, challengeType: `string`, challengeMetadata: `string`)

### `Class.GenericChallengeService.ChallengeInvalidatedEvent`

Fires with: (challengeID: `string`)

### `Class.GenericChallengeService.ChallengeLoadedEvent`

Fires with: (challengeID: `string`, success: `bool`)

### `Class.GenericChallengeService.ChallengeRequiredEvent`

Fires with: (challengeID: `string`, challengeType: `string`, challengeMetadata: `string`)
