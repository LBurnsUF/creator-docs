---
title: Annotation
type: class
superclass: Instance
---

# Annotation

**Inherits**: Instance > Object

## Properties

- **AuthorColor3**: `Color3` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **AuthorId**: `int64` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **ChannelId**: `string` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Contents**: `string` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **CreationTimeUnix**: `int64` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **LastModifiedTimeUnix**: `int64` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **LoadingReplies**: `bool` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **ReplyCount**: `int64` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Resolved**: `bool` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **TaggedUsers**: `string` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **GetRequests**() -> `Dictionary`
- **GetStringUniqueId**() -> `string`
- **IsThreadParent**() -> `bool`

## Events

- **RequestCompleted**(`requestId: string`, `requestType: AnnotationRequestType`, `result: AnnotationRequestStatus`)
- **RequestInitiated**(`requestId: string`, `requestType: AnnotationRequestType`)
