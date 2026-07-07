---
title: SocialService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# SocialService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.SocialService:CanSendCallInviteAsync`

``CanSendCallInviteAsync(player: `Class.Instance`)`` → `bool`
  [Yields]

### `Class.SocialService:CanSendGameInviteAsync`

``CanSendGameInviteAsync(player: `Class.Instance`, recipientId: `Datatype.User`)`` → `bool`
  [Yields]

### `Class.SocialService:GetEventRsvpStatusAsync`

``GetEventRsvpStatusAsync(eventId: `string`)`` → `Enum.RsvpStatus`
  [Yields]

### `Class.SocialService:GetExperienceEventAsync`

``GetExperienceEventAsync(eventId: `string`)`` → `Dictionary?`
  [Yields]

### `Class.SocialService:GetPartyAsync`

``GetPartyAsync(partyId: `string`)`` → `Array`
  [Yields]

### `Class.SocialService:GetPlayersByPartyId`

``GetPlayersByPartyId(partyId: `string`)`` → `Datatype.Instances`

### `Class.SocialService:GetUpcomingExperienceEventsAsync`

``GetUpcomingExperienceEventsAsync()`` → `Array`
  [Yields]

### `Class.SocialService:HideSelfView`

``HideSelfView()`` → `null`

### `Class.SocialService:InvokeGameInvitePromptClosed`

``InvokeGameInvitePromptClosed(player: `Class.Instance`, recipientIds: `Array`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SocialService:InvokeIrisInvite`

``InvokeIrisInvite(player: `Class.Instance`, tag: `string`, irisParticipants: `Array`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SocialService:InvokeIrisInvitePromptClosed`

``InvokeIrisInvitePromptClosed(player: `Class.Instance`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SocialService:InvokeShareSheetClosed`

``InvokeShareSheetClosed()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SocialService:PromptFeedbackSubmissionAsync`

``PromptFeedbackSubmissionAsync(options: `Dictionary?`)`` → `null`
  [Yields]

### `Class.SocialService:PromptGameInvite`

``PromptGameInvite(player: `Class.Instance`, experienceInviteOptions: `Class.Instance`)`` → `null`

### `Class.SocialService:PromptLinkSharing`

``PromptLinkSharing(player: `Class.Player`, options: `Dictionary`)`` → `Tuple`
  [Yields] [Deprecated]

### `Class.SocialService:PromptLinkSharingAsync`

``PromptLinkSharingAsync(player: `Class.Player`, options: `Dictionary`)`` → `Tuple`
  [Yields]

### `Class.SocialService:PromptPhoneBook`

``PromptPhoneBook(player: `Class.Instance`, tag: `string`)`` → `null`

### `Class.SocialService:PromptRsvpToEventAsync`

``PromptRsvpToEventAsync(eventId: `string`)`` → `Enum.RsvpStatus`
  [Yields]

### `Class.SocialService:PromptRsvpToEventCompleted`

``PromptRsvpToEventCompleted(eventId: `string`, success: `bool`, rsvpStatus: `Enum.RsvpStatus`, previousRsvpStatus: `Enum.RsvpStatus`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SocialService:ShowSelfView`

``ShowSelfView(selfViewPosition: `Enum.SelfViewPosition`)`` → `null`

### `Class.SocialService:SignalFeedbackSubmissionCompleted`

``SignalFeedbackSubmissionCompleted(feedback: `string`, options: `Dictionary?`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SocialService:SignalFeedbackSubmissionPermissionDenied`

``SignalFeedbackSubmissionPermissionDenied()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.SocialService:UpdatePlayerPartyData`

``UpdatePlayerPartyData(partyId: `string`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.SocialService.CallInviteStateChanged`

Fires with: (player: `Class.Instance`, inviteState: `Enum.InviteState`)

### `Class.SocialService.GameInvitePromptClosed`

Fires with: (player: `Class.Instance`, recipientIds: `Array`)

### `Class.SocialService.OpenShareSheetWithLink`

Fires with: (link: `string`)

### `Class.SocialService.PhoneBookPromptClosed`

Fires with: (player: `Class.Instance`)

### `Class.SocialService.PlayerPartyDataChanged`

Fires with: (partyId: `string`)

### `Class.SocialService.PromptInviteRequested`

Fires with: (player: `Class.Instance`, experienceInviteOptions: `Class.Instance`)

### `Class.SocialService.PromptIrisInviteRequested`

Fires with: (player: `Class.Instance`, tag: `string`)

### `Class.SocialService.SelfViewHidden`

Fires with: ()

### `Class.SocialService.SelfViewVisible`

Fires with: (selfViewPosition: `Enum.SelfViewPosition`)

### `Class.SocialService.ShareSheetClosed`

Fires with: (player: `Class.Player`)

### `Class.SocialService.ShowPromptFeedbackSubmission`

Fires with: (feedbackType: `Enum.FeedbackType`)

### `Class.SocialService.ShowPromptFeedbackUnavailable`

Fires with: (reason: `string`, feedbackType: `Enum.FeedbackType`)

### `Class.SocialService.ShowPromptRsvpToEvent`

Fires with: (eventId: `string`)

## Callbacks

### `Class.SocialService.OnCallInviteInvoked`

``OnCallInviteInvoked(tag: `string`, callParticipantIds: `Array`)`` → `Class.Instance`
