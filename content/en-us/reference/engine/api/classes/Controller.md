---
title: Controller
type: class
superclass: Instance
tags: [NotCreatable]
---

# Controller

The base class for controller objects, such as the `Class.HumanoidController`
object.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

The base class for controller objects, such as the `Class.HumanoidController`
object.

## Methods

### `Class.Controller:BindButton`

``BindButton(button: `Enum.Button`, caption: `string`)`` -> `null`

### `Class.Controller:GetButton`

``GetButton(button: `Enum.Button`)`` -> `bool`

### `Class.Controller:UnbindButton`

``UnbindButton(button: `Enum.Button`)`` -> `null`

### `Class.Controller:bindButton`

``bindButton(button: `Enum.Button`, caption: `string`)`` -> `null`
  [Deprecated]

### `Class.Controller:getButton`

``getButton(button: `Enum.Button`)`` -> `bool`
  [Deprecated]

## Events

### `Class.Controller.ButtonChanged`

Fires with: (button: `Enum.Button`)
