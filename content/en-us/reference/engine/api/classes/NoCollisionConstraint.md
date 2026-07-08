---
title: NoCollisionConstraint
type: class
superclass: Instance
---

# NoCollisionConstraint

An instance used to prevent collisions between two specific parts.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

The **NoCollisionConstraint** prevents collisions between two specific parts,
but those parts may still register collisions with the rest of the world.
Compared to
[collision groups](../../../workspace/collisions.md#collision-filtering), it
provides a direct way to disable specific collisions, such as the wheel of a
car scraping against the car's body.

The most common way to create this constraint is by selecting
**No&nbsp;Collision** through Studio's **Create** menu in the toolbar's
**Model** tab.

Unlike most constraints, `Class.NoCollisionConstraint` does not utilize any
`Class.Attachment|Attachments`. Note that the tool acts differently based on
how many parts are selected when the tool is activated:

<table>
<thead>
  <tr>
    <td>Option</td>
    <td>Tool Behavior</td>
  </tr>
</thead>
<tbody>
  <tr>
    <td>No parts selected</td>
    <td>The next two parts that are clicked will be linked together. If the same part is clicked twice, no link will be created.</td>
  </tr>
  <tr>
    <td>One part selected</td>
    <td>The next part that is clicked will be linked to the selected part.</td>
  </tr>
  <tr>
    <td>Two parts selected</td>
    <td>Both selected parts will be linked together.</td>
  </tr>
</tbody>
</table>

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.NoCollisionConstraint.Enabled` | `bool` |  |
| `Class.NoCollisionConstraint.Part0` | `Class.BasePart` |  |
| `Class.NoCollisionConstraint.Part1` | `Class.BasePart` |  |
