---
title: Highlight
type: class
superclass: Instance
---

# Highlight

A visual effect which you can use to call attention to a specific object
within an experience.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

The `Class.Highlight` instance is a visual effect which you can use to call
attention to a specific object within an experience. Every highlight effect
has a silhouette **outline** that surrounds the object and a solid overlay
**interior** that displays over the object. You can customize both of these
components independently to modify the highlight's visual appearance.

<table size="small">
  <tbody>
    <tr>
      <td width="30%">
        <figure>
        <img src="/assets/ui/highlighting-objects/OutlineTransparency-1.jpg" />
        <figcaption>Base object</figcaption>
        </figure>
      </td>
      <td width="30%">
        <figure>
        <img src="/assets/ui/highlighting-objects/Adding-Highlight.jpg" />
        <figcaption>White outline, 50% red interior</figcaption>
        </figure>
      </td>
      <td width="30%">
        <figure>
        <img src="/assets/ui/highlighting-objects/Overview-Yellow-Outline.jpg" />
        <figcaption>Yellow outline, black interior</figcaption>
        </figure>
      </td>
    </tr>
  </tbody>
</table>

Useful applications of the highlight effect include:

- Providing visual feedback that an object is important and/or interactable.
- Making distant objects visible through objects that are closer to the user.
- Indicating the current position and status of other characters.

#### Limitations

As a performance limit, Studio only displays 255 simultaneous
`Class.Highlight` instances on the client at a time. If you exceed this limit,
the additional instances are silently ignored. Note that while a
`Class.Highlight` with `Class.Highlight.Enabled|Enabled` set to `false`
doesn't display, it still takes one of the 255 available slots, so if you plan
to permanently disable a `Class.Highlight` instance, it's best to delete it
rather than disable it.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Highlight.Adornee` | `Class.Instance` |  |
| `Class.Highlight.DepthMode` | `Enum.HighlightDepthMode` |  |
| `Class.Highlight.Enabled` | `bool` |  |
| `Class.Highlight.FillColor` | `Datatype.Color3` |  |
| `Class.Highlight.FillTransparency` | `float` |  |
| `Class.Highlight.LineThickness` | `int` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.Highlight.OutlineColor` | `Datatype.Color3` |  |
| `Class.Highlight.OutlineTransparency` | `float` |  |
| `Class.Highlight.ReservedId` | `Enum.ReservedHighlightId` | [Hidden] {security: RobloxScriptSecurity} |
