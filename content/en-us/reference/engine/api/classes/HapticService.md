---
title: HapticService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# HapticService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.HapticService:GetMotor`

``GetMotor(inputType: `Enum.UserInputType`, vibrationMotor: `Enum.VibrationMotor`)`` → `Tuple`

### `Class.HapticService:IsMotorSupported`

``IsMotorSupported(inputType: `Enum.UserInputType`, vibrationMotor: `Enum.VibrationMotor`)`` → `bool`

### `Class.HapticService:IsVibrationSupported`

``IsVibrationSupported(inputType: `Enum.UserInputType`)`` → `bool`

### `Class.HapticService:SetMotor`

``SetMotor(inputType: `Enum.UserInputType`, vibrationMotor: `Enum.VibrationMotor`, vibrationValues: `Tuple`)`` → `null`
