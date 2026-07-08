---
title: PackageLink
type: class
superclass: Instance
tags: [NotCreatable, NotBrowsable]
---

# PackageLink

Links a `Class.DataModel` instance to a corresponding asset in the cloud.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotBrowsable]

## Description

The purpose of the `Class.PackageLink` object is to link a `Class.DataModel`
instance to a corresponding asset in the cloud. This improves flows for
collaboration, version control, and sharing for models. The
`Class.PackageLink` instance will be a child of the root of the entire package
hierarchy.

`Class.PackageLink|PackageLinks` are not creatable through
`Class.Script|Scripts`. They can only be added through interaction with Studio
and can only be parented to `Class.Instance|Instances` that can be published
independently of `Class.DataModel` publish. The `Class.PackageLink` instance
will always be the first child shown in the tree view, regardless of sorting.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.PackageLink.AutoUpdate` | `bool` |  {security: RobloxScriptSecurity} |
| `Class.PackageLink.Creator` | `string` | [ReadOnly] [NotReplicated] [NotScriptable] |
| `Class.PackageLink.DefaultName` | `string` |  {write: NotAccessibleSecurity} |
| `Class.PackageLink.HasNewVersion` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.PackageLink.ModifiedState` | `int` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.PackageLink.PackageAssetName` | `string` | [ReadOnly] [NotReplicated] [NotScriptable] |
| `Class.PackageLink.PackageContent` | `Datatype.Content` | [ReadOnly] [NotReplicated] |
| `Class.PackageLink.PackageId` | `Datatype.ContentId` | [ReadOnly] [NotReplicated] |
| `Class.PackageLink.PermissionLevel` | `Enum.PackagePermission` | [ReadOnly] [NotReplicated] [NotScriptable] |
| `Class.PackageLink.SerializedDefaultAttributes` | `Datatype.BinaryString` |  {write: NotAccessibleSecurity} |
| `Class.PackageLink.Status` | `string` | [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.PackageLink.VersionNumber` | `int64` | [NotReplicated] {write: NotAccessibleSecurity} |
