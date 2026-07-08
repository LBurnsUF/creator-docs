---
title: UIPageLayout
type: class
superclass: UIGridStyleLayout
---

# UIPageLayout

**Inherits from:** `Class.UIGridStyleLayout` > `Class.UILayout` > `Class.UIComponent` > `Class.UIBase` > `Class.Instance` > `Class.Object`

## Description

Creates a paged viewing window, like the home screen of a mobile device. You
can use a UIPageLayout by parenting it to a GuiObject. The UIPageLayout will
then apply itself to all of its GuiObject siblings.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.UIPageLayout.Animated` | `bool` |  |
| `Class.UIPageLayout.Circular` | `bool` |  |
| `Class.UIPageLayout.CurrentPage` | `Class.GuiObject` | [ReadOnly] [NotReplicated] |
| `Class.UIPageLayout.EasingDirection` | `Enum.EasingDirection` |  |
| `Class.UIPageLayout.EasingStyle` | `Enum.EasingStyle` |  |
| `Class.UIPageLayout.GamepadInputEnabled` | `bool` |  |
| `Class.UIPageLayout.Padding` | `Datatype.UDim` |  |
| `Class.UIPageLayout.ScrollWheelInputEnabled` | `bool` |  |
| `Class.UIPageLayout.TouchInputEnabled` | `bool` |  |
| `Class.UIPageLayout.TweenTime` | `float` |  |

## Methods

### `Class.UIPageLayout:JumpTo`

``JumpTo(page: `Class.Instance`)`` -> `null`

### `Class.UIPageLayout:JumpToIndex`

``JumpToIndex(index: `int`)`` -> `null`

### `Class.UIPageLayout:Next`

``Next()`` -> `null`

### `Class.UIPageLayout:Previous`

``Previous()`` -> `null`

## Events

### `Class.UIPageLayout.PageEnter`

Fires with: (page: `Class.Instance`)

### `Class.UIPageLayout.PageLeave`

Fires with: (page: `Class.Instance`)

### `Class.UIPageLayout.Stopped`

Fires with: (currentPage: `Class.Instance`)
