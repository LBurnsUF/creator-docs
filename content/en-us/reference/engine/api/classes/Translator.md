---
title: Translator
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# Translator

The role of a Translator is to manufacture/return strings localized for the
viewing player.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

The role of a Translator is to manufacture/return strings localized for the
viewing player. It can be used to retrieve display-ready localized text from a
`Class.LocalizationTable`. The source of the `Class.Translator.LocaleId`
property, the set of tables it will search, and the order it will search them
in depends on which method was used to create the Translator instance.

The input for a Translator is the original development language string and a
context, where all or part of the context can be used to find a more
precise/situational translation for the source string.

The Translator can also be used to manufacture translated strings with inserts
(data replacements) which may change order based on the target language.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Translator.LocaleId` | `string` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.Translator:FormatByKey`

``FormatByKey(key: `string`, args: `Variant`)`` -> `string`

### `Class.Translator:RobloxOnlyTranslate`

``RobloxOnlyTranslate(context: `Class.Instance`, text: `string`)`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.Translator:Translate`

``Translate(context: `Class.Instance`, text: `string`)`` -> `string`
