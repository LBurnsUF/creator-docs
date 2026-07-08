---
title: Rotate
type: class
superclass: JointInstance
tags: [Deprecated]
---

# Rotate

**Inherits from:** `Class.JointInstance` > `Class.Instance` > `Class.Object`

**Tags:** [Deprecated]

## Description

The **Rotate** object is used to allow rotation between two parts. Most
commonly created through the `Enum.SurfaceType.Hinge` on a `Class.BasePart`.
If created like this, the rotation will be about the normal vector from the
face of the part the hinge is placed on. If created through a script, the axis
and point of rotation can be defined arbitrarily.

> **Deprecated:** This class works alongside the deprecated `Enum.SurfaceType` and should not be
used for future work; use `Class.HingeConstraint` instead.
