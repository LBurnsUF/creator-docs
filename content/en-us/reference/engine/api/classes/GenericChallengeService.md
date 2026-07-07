---
title: GenericChallengeService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# GenericChallengeService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **SignalChallengeAbandoned**(`challengeID: string`) -> `null`
- **SignalChallengeCompleted**(`challengeID: string`, `challengeType: string`, `challengeMetadata: string`) -> `null`
- **SignalChallengeInvalidated**(`challengeID: string`) -> `null`
- **SignalChallengeLoaded**(`challengeID: string`, `success: bool`) -> `null`
- **SignalChallengeRequired**(`challengeID: string`, `challengeType: string`, `challengeMetadata: string`) -> `null`

## Events

- **ChallengeAbandonedEvent**(`challengeID: string`)
- **ChallengeCompletedEvent**(`challengeID: string`, `challengeType: string`, `challengeMetadata: string`)
- **ChallengeInvalidatedEvent**(`challengeID: string`)
- **ChallengeLoadedEvent**(`challengeID: string`, `success: bool`)
- **ChallengeRequiredEvent**(`challengeID: string`, `challengeType: string`, `challengeMetadata: string`)
