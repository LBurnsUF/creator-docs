---
title: AnimationRigData
type: class
superclass: Instance
---

# AnimationRigData

Used to store information regarding the model an animation was authored for.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

An AnimationRigData instance commonly appears in the Data Model as a child of
an AnimationClip. It is used to store information regarding the source rig an
animation was authored for. It is currently only used for AnimationClips
authored on R15 rigs.

## Methods

### `Class.AnimationRigData:GetLabels`

``GetLabels()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.AnimationRigData:GetNames`

``GetNames()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.AnimationRigData:GetParents`

``GetParents()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.AnimationRigData:GetPostTransforms`

``GetPostTransforms()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.AnimationRigData:GetPreTransforms`

``GetPreTransforms()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.AnimationRigData:GetTransforms`

``GetTransforms()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.AnimationRigData:IsValidR15`

``IsValidR15()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.AnimationRigData:IsValidR15Plus`

``IsValidR15Plus()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.AnimationRigData:LoadFromHumanoid`

``LoadFromHumanoid(humanoid: `Class.Instance`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.AnimationRigData:LoadFromModel`

``LoadFromModel(model: `Class.Instance`)`` -> `bool`
   {security: RobloxScriptSecurity}
