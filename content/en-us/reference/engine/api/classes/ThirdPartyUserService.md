---
title: ThirdPartyUserService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ThirdPartyUserService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **FriendCommunicationRestrictionStatus**: `ChatRestrictionStatus` [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **HasActiveUser**: `bool` [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **VoiceChatRestrictionStatus**: `ChatRestrictionStatus` [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **GetUserPlatformName**() -> `string`
- **GetVoiceChatRestrictionStatus**() -> `ChatRestrictionStatus`
- **HaveActiveUser**() -> `bool`
- **IsAccountSwitchingSupported**() -> `bool`
- **IsChatRestrictionSupported**() -> `bool`
- **IsSingleSignOnSupported**() -> `bool`
- **RegisterActiveUser**(`gamepadId: UserInputType`) -> `int` [Yields]
- **ShowAccountPicker**() -> `null`

## Events

- **ActiveUserSignedOut**(`signOutStatus: int`)
