---
title: StudioTestService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# StudioTestService

Service allowing plugins to automate and customize Test and Run mode testing.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

`StudioTestService` allows plugins to automate and customize Test and Run mode
testing. With `StudioTestService`, your plugins can launch tests that jump
straight to a specific part of your game, or run complex code tests
automatically.

You can use `StudioTestService` to start a server with multiple simulated
clients, add players mid-session, pass arguments into running tests, end tests
from the server, and trigger client disconnections, all without manually
clicking through the Test tab in Studio.

These methods complement the existing playtest automation available through
Studio's built-in MCP server. Where the MCP server's `start_stop_play` tool
starts a single Play Client session, the `StudioTestService` methods are
designed for scripted multi-client scenarios such as lobby, matchmaking, and
join/leave flow testing.

A typical multiplayer test splits across three script contexts: the plugin
that launches it, the server that drives it, and the clients that participate:

Plugin script:

```lua
local StudioTestService = game:GetService("StudioTestService")

local toolbar = plugin:CreateToolbar("STS Tests")
local button = toolbar:CreateButton("MyTest", "", "")

button.Click:Connect(function()
    button.Enabled = false
    local result = StudioTestService:ExecuteMultiplayerTestAsync(1, "MyArguments")
    assert(result == "Success!")
    print("Test finished successfully!")
    button.Enabled = true
end)
```

Server script:

```lua
local Players = game:GetService("Players")
local StudioTestService = game:GetService("StudioTestService")

assert(StudioTestService:GetTestArgs() == "MyArguments")

Players.PlayerRemoving:Connect(function(player)
    print(player.Name .. " left the experience")
    task.wait(3)
    StudioTestService:EndTest("Success!")
end)
```

Client script:

```lua
if not game:IsLoaded() then
    game.Loaded:Wait()
end

local StudioTestService = game:GetService("StudioTestService")
task.wait(3)
StudioTestService:LeaveTest()
```

##### Limitations

- `ExecuteMultiplayerTestAsync` can only be called from plugin scripts. It
  yields until the test ends, so wrap it in a coroutine if the calling plugin
  needs to remain responsive.
- `ExecuteMultiplayerTestAsync` cannot be called from inside a running test.
- `ExecuteMultiplayerTestAsync` supports up to 8 simulated clients per test
  session.
- Only one multiplayer test session can run at a time per Studio instance.
- `AddPlayers` and `EndTest` must be called from the server DataModel of a
  running test.
- `CanLeaveTest` and `LeaveTest` must be called from a client DataModel.
- `GetTestArgs` currently has a known issue when called from a client
  LocalScript.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.StudioTestService.EditModeActive` | `bool` |  {security: PluginSecurity} |

## Methods

### `Class.StudioTestService:AddPlayers`

``AddPlayers(numPlayers: `int`)`` -> `null`

### `Class.StudioTestService:CanLeaveTest`

``CanLeaveTest()`` -> `bool`

### `Class.StudioTestService:EndTest`

``EndTest(value: `Variant`)`` -> `null`

### `Class.StudioTestService:ExecuteMultiplayerTestAsync`

``ExecuteMultiplayerTestAsync(numPlayers: `int`, args: `Variant`)`` -> `Variant`
  [Yields] {security: PluginSecurity}

### `Class.StudioTestService:ExecutePlayModeAsync`

``ExecutePlayModeAsync(args: `Variant`)`` -> `Variant`
  [Yields] {security: PluginSecurity}

### `Class.StudioTestService:ExecuteRunModeAsync`

``ExecuteRunModeAsync(args: `Variant`)`` -> `Variant`
  [Yields] {security: PluginSecurity}

### `Class.StudioTestService:GetTestArgs`

``GetTestArgs()`` -> `Variant`

### `Class.StudioTestService:LeaveTest`

``LeaveTest()`` -> `null`
