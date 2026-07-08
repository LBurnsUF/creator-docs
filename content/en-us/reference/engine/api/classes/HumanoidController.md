---
title: HumanoidController
type: class
superclass: Controller
---

# HumanoidController

**Inherits from:** `Class.Controller` > `Class.Instance` > `Class.Object`

## Description

A HumanoidController is an internal object responsible for translating
PlayerAction movements to the user's character (specifically, their
`Class.Humanoid`).

This object can be found inside of the `Class.ControllerService`, via:

```lua
local ControllerService = game:GetService("ControllerService")
local HumanoidController = ControllerService:FindFirstChildOfClass("HumanoidController")
```
