---
title: Dragger
type: class
superclass: Instance
---

# Dragger

A helper object used to create tools that can drag parts.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

The **Dragger** object is a helper object used to create tools that can drag
parts. It is expected (but not required) to be used with `Class.Mouse` events.

Its implementation is primarily used in the RbxStamper library.

> **Deprecated:** This class has been deprecated, as it does not work well with
`Class.Workspace.FilteringEnabled|FilteringEnabled`, and should not be used in
new work.

## Methods

### `Class.Dragger:AxisRotate`

``AxisRotate(axis: `Enum.Axis`)`` -> `null`

### `Class.Dragger:MouseDown`

``MouseDown(mousePart: `Class.Instance`, pointOnMousePart: `Datatype.Vector3`, parts: `Datatype.Instances`)`` -> `null`

### `Class.Dragger:MouseMove`

``MouseMove(mouseRay: `Datatype.Ray`)`` -> `null`

### `Class.Dragger:MouseUp`

``MouseUp()`` -> `null`
