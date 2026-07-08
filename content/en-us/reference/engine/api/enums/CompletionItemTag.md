---
title: CompletionItemTag
type: enum
---

# `Enum.CompletionItemTag`

Determines the tags for completion items in
`Class.ScriptEditorService:RegisterAutocompleteCallback()`.

Determines the tags for completion items in
`Class.ScriptEditorService:RegisterAutocompleteCallback()`.

The `Enum.CompletionItemTag` enum has 11 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.CompletionItemTag.Deprecated` | 1 | Indicates that the completion is deprecated, applying a penalty towards its score and crossing it ou |
| `Enum.CompletionItemTag.IncorrectIndexType` | 2 | Indicates that the completion is a member and being accessed with the wrong index type (e.g. using ` |
| `Enum.CompletionItemTag.PluginPermissions` | 3 | Indicates that the completion requires Plugin security level to access, hiding it if the client lack |
| `Enum.CompletionItemTag.CommandLinePermissions` | 4 | Indicates that the completion requires Command line security level to access, hiding it if the clien |
| `Enum.CompletionItemTag.RobloxPermissions` | 5 | Indicates that the completion requires core script security level to access, hiding it if the client |
| `Enum.CompletionItemTag.AddParens` | 6 | Instructs the editor to add parentheses before the cursor after inserting the given completion, if a |
| `Enum.CompletionItemTag.PutCursorInParens` | 7 | Instructs the editor to add parentheses before the cursor and move the cursor into the parentheses a |
| `Enum.CompletionItemTag.TypeCorrect` | 8 | Indicates that the completion is type correct in the current context, granting a bonus to its score. |
| `Enum.CompletionItemTag.ClientServerBoundaryViolation` | 9 | Indicates that the completion is being accessed from the wrong side of the client/server boundary (e |
| `Enum.CompletionItemTag.Invalidated` | 10 |  |
| `Enum.CompletionItemTag.PutCursorBeforeEnd` | 11 |  |
