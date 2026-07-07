---
title: HapticService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# HapticService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **GetMotor**(`inputType: UserInputType`, `vibrationMotor: VibrationMotor`) -> `Tuple`
- **IsMotorSupported**(`inputType: UserInputType`, `vibrationMotor: VibrationMotor`) -> `bool`
- **IsVibrationSupported**(`inputType: UserInputType`) -> `bool`
- **SetMotor**(`inputType: UserInputType`, `vibrationMotor: VibrationMotor`, `vibrationValues: Tuple`) -> `null`
