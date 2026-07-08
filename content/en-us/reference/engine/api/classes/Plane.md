---
title: Plane
type: class
superclass: PlaneConstraint
tags: [Deprecated]
---

# Plane

Constrains Attachment0 and Attachment1 such that both points lie in a plane
with origin at Attachment0's position and unit normal vector equal to
Attachment0's primary axis.

**Inherits from:** `Class.PlaneConstraint` > `Class.Constraint` > `Class.Instance` > `Class.Object`

**Tags:** [Deprecated]

## Description

Constrains Attachment0 and Attachment1 such that both points lie in a plane
defined by Attachment0. The plane origin is at Attachment0 and the plane unit
normal is the primary axis of Attachment0. This means that Attachment0 and
Attachment1 will move to a position/orientation such that the distance between
Attachment1 and Attachment0, projected onto the Plane unit normal, is zero.
