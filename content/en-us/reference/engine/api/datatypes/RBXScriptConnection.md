---
title: RBXScriptConnection
type: datatype
---

# `Datatype.RBXScriptConnection`

A connection between an `Datatype.RBXScriptSignal` and a function.

## Description

The `RBXScriptConnection` data type is a special object returned by the
`Datatype.RBXScriptSignal:Connect()|Connect()` method of an event
(`Datatype.RBXScriptSignal`). This is used primarily to disconnect a listener
from an `Datatype.RBXScriptSignal`.

```lua
local part : BasePart = script.Parent
-- Store reference to the RBXScriptConnection so it can be disconnected later
local connection : RBXScriptConnection = part.Touched:Connect(function(otherPart)
    print("Hello world!")
end)
-- Wait 15 seconds, then disconnect
task.wait(15)
connection:Disconnect()
```

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `RBXScriptConnection.Connected` | `bool` | The state of the RBXScriptConnection. |

## Methods

### `RBXScriptConnection:Disconnect`

Disconnects the connection from the event.

## API Usage (14 locations)

### Used as Return Type

- `Class.Actor:BindToMessage`
- `Class.Actor:BindToMessageParallel`
- `Class.DragDetector:AddConstraintFunction`
- `Class.ExperienceService:RegisterForExperienceJoin`
- `Class.ExperienceService:RegisterForExperienceLeave`
- `Class.GlobalDataStore:OnUpdate`
- `Class.MarketplaceService:BindReceiptHandler`
- `Class.MessagingService:SubscribeAsync`
- `Class.ModerationService:BindReviewableContentEventProcessor`
- `Class.PluginConnection:BindToMessage`
- `Class.RunService:BindToSimulation`
- `Class.Selection:AddFocusCallback`
- `Class.StudioPublishService:RegisterPublishHold`
- `Class.UIDragDetector:AddConstraintFunction`
