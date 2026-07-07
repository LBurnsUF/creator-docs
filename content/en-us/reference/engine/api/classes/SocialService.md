---
title: SocialService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# SocialService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **CanSendCallInviteAsync**(`player: Instance`) -> `bool` [Yields]
- **CanSendGameInviteAsync**(`player: Instance`, `recipientId: User = U1.AQAAAAAAAAAAAAAAAAAAAAA`) -> `bool` [Yields]
- **GetEventRsvpStatusAsync**(`eventId: string`) -> `RsvpStatus` [Yields]
- **GetExperienceEventAsync**(`eventId: string`) -> `Dictionary?` [Yields]
- **GetPartyAsync**(`partyId: string`) -> `Array` [Yields]
- **GetPlayersByPartyId**(`partyId: string`) -> `Instances`
- **GetUpcomingExperienceEventsAsync**() -> `Array` [Yields]
- **HideSelfView**() -> `null`
- **InvokeGameInvitePromptClosed**(`player: Instance`, `recipientIds: Array`) -> `null`
- **InvokeIrisInvite**(`player: Instance`, `tag: string`, `irisParticipants: Array`) -> `null`
- **InvokeIrisInvitePromptClosed**(`player: Instance`) -> `null`
- **InvokeShareSheetClosed**() -> `null`
- **PromptFeedbackSubmissionAsync**(`options: Dictionary?`) -> `null` [Yields]
- **PromptGameInvite**(`player: Instance`, `experienceInviteOptions: Instance = nil`) -> `null`
- **PromptLinkSharing**(`player: Player`, `options: Dictionary = nil`) -> `Tuple` [Yields] [Deprecated]
- **PromptLinkSharingAsync**(`player: Player`, `options: Dictionary = nil`) -> `Tuple` [Yields]
- **PromptPhoneBook**(`player: Instance`, `tag: string`) -> `null`
- **PromptRsvpToEventAsync**(`eventId: string`) -> `RsvpStatus` [Yields]
- **PromptRsvpToEventCompleted**(`eventId: string`, `success: bool`, `rsvpStatus: RsvpStatus`, `previousRsvpStatus: RsvpStatus = None`) -> `null`
- **ShowSelfView**(`selfViewPosition: SelfViewPosition = LastPosition`) -> `null`
- **SignalFeedbackSubmissionCompleted**(`feedback: string`, `options: Dictionary?`) -> `null`
- **SignalFeedbackSubmissionPermissionDenied**() -> `null`
- **UpdatePlayerPartyData**(`partyId: string`) -> `null`

## Events

- **CallInviteStateChanged**(`player: Instance`, `inviteState: InviteState`)
- **GameInvitePromptClosed**(`player: Instance`, `recipientIds: Array`)
- **OpenShareSheetWithLink**(`link: string`)
- **PhoneBookPromptClosed**(`player: Instance`)
- **PlayerPartyDataChanged**(`partyId: string`)
- **PromptInviteRequested**(`player: Instance`, `experienceInviteOptions: Instance`)
- **PromptIrisInviteRequested**(`player: Instance`, `tag: string`)
- **SelfViewHidden**()
- **SelfViewVisible**(`selfViewPosition: SelfViewPosition`)
- **ShareSheetClosed**(`player: Player`)
- **ShowPromptFeedbackSubmission**(`feedbackType: FeedbackType`)
- **ShowPromptFeedbackUnavailable**(`reason: string`, `feedbackType: FeedbackType`)
- **ShowPromptRsvpToEvent**(`eventId: string`)

## Callbacks

- **OnCallInviteInvoked**(`tag: string`, `callParticipantIds: Array`) -> `Instance`
