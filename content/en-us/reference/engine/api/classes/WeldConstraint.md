---
title: WeldConstraint
type: class
superclass: Instance
---

# WeldConstraint

Connects two `Class.BasePart|BaseParts` together such that their relative
position and orientation remain the same.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

**WeldConstraint** connects two `Class.BasePart|BaseParts` and ensures they
stay in the same relative position/orientation to each other, meaning that if
one part moves, the other moves the same amount. Even if the two parts are not
touching, they can be welded together.

The most common way to create a weld constraint is by selecting **Weld**
through Studio's **Create** menu in the toolbar's **Model** tab.

Note that this tool behaves differently depending on how many
`Class.BasePart|BaseParts` are selected when the tool is activated:

- If no `Class.BasePart|BaseParts` are selected, the next two
  `Class.BasePart|BaseParts` clicked will be connected by a new
  `Class.WeldConstraint`. If the same `Class.BasePart` is clicked twice, no
  constraint will be created.
- If one `Class.BasePart` is already selected, the next `Class.BasePart`
  clicked will be connected to the selected one with a new
  `Class.WeldConstraint`.
- If multiple `Class.BasePart|BaseParts` are selected, those which are
  touching or overlapping will be automatically welded together by new
  `Class.WeldConstraint|WeldConstraints`.

#### Repositioning Behavior

Moving a welded `Class.BasePart` behaves differently depending on whether the
part was moved through its `Class.BasePart.Position|Position` or through its
`Datatype.CFrame`.

- If a welded part's `Class.BasePart.Position|Position` is updated, that part
  will move but none of the connected parts will move with it. The weld will
  recalculate the offset from the other parts based on the moved part's new
  position.

- If a welded part's `Datatype.CFrame` is updated, that part will move **and**
  all of the connected parts will also move, ensuring they maintain the same
  offset as when the weld was created.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.WeldConstraint.Active` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.WeldConstraint.Enabled` | `bool` | [NotReplicated] |
| `Class.WeldConstraint.Part0` | `Class.BasePart` | [NotReplicated] |
| `Class.WeldConstraint.Part1` | `Class.BasePart` | [NotReplicated] |
