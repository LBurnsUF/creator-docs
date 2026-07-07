---
title: Translator
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# Translator

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.Translator.LocaleId` | `string` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.Translator:FormatByKey`

``FormatByKey(key: `string`, args: `Variant`)`` → `string`

### `Class.Translator:RobloxOnlyTranslate`

``RobloxOnlyTranslate(context: `Class.Instance`, text: `string`)`` → `string`
   {security: RobloxScriptSecurity}

### `Class.Translator:Translate`

``Translate(context: `Class.Instance`, text: `string`)`` → `string`
