---
title: JointInstance
type: class
superclass: Instance
tags: [NotCreatable]
---

# JointInstance

The base class for joints.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

`JointInstance` is the base class for joints such as `Class.Weld|Welds` and
`Class.Motor|Motors`.

`Class.Weld`, `Class.WeldConstraint`, `Class.Motor`, and `Class.Motor6D` all
combine multiple parts into the same
[assembly](../../../physics/assemblies.md). Every assembly has a root part
(`Class.BasePart:GetRootPart()`) and when
`Class.JointInstance.C0|C0`/`Class.JointInstance.C1|C1` of a
`Class.JointInstance` is modified, the root part will stay where it was.

Welds do not have any directionality. You can imagine rigid joints forming a
tree branching down from the root part. All the parts down the tree from root
will move, and their welded "children" in this tree will move with them.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.JointInstance.Active` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.JointInstance.C0` | `Datatype.CFrame` |  |
| `Class.JointInstance.C1` | `Datatype.CFrame` |  |
| `Class.JointInstance.Enabled` | `bool` |  |
| `Class.JointInstance.Part0` | `Class.BasePart` |  |
| `Class.JointInstance.Part1` | `Class.BasePart` |  |
| `Class.JointInstance.part1` | `Class.BasePart` | [Hidden] [NotReplicated] [Deprecated] |
