---
title: UIFlexItem
type: class
superclass: UIComponent
---

# UIFlexItem

Defines flex behavior for a `Class.GuiObject` within a `Class.UIListLayout`.

**Inherits from:** `Class.UIComponent` > `Class.UIBase` > `Class.Instance` > `Class.Object`

## Description

The `Class.UIFlexItem` object defines flex behavior for its parent
`Class.GuiObject` under the control of a `Class.UIListLayout`. The defined
flex behavior overrides that of the controlling `Class.UIListLayout`, letting
you configure flex behavior on a per‑object basis where necessary.

<img src="../../../assets/ui/ui-objects/UIFlexItem-Example.png" width="720" alt="Example of UIFlexItem applied to a specific GuiObject under control of a UIListLayout." />

<img src="../../../assets/ui/ui-objects/UIFlexItem-Hierarchy.png" width="500" alt="Example hierarchy of a UIFlexItem parented to a GuiObject under control of a UIListLayout." />

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.UIFlexItem.FlexMode` | `Enum.UIFlexMode` |  |
| `Class.UIFlexItem.GrowRatio` | `float` |  |
| `Class.UIFlexItem.ItemLineAlignment` | `Enum.ItemLineAlignment` |  |
| `Class.UIFlexItem.ShrinkRatio` | `float` |  |
