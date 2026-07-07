---
title: ExplorerFilter
type: class
superclass: Instance
tags: [NotReplicated]
---

# ExplorerFilter

**Inherits**: Instance > Object

**Tags**: NotReplicated

## Methods

- **BeginSearch**(`root: Instance`) -> `null`
- **GetAutocompleter**() -> `ExplorerFilterAutocompleter`
- **GetErrors**() -> `Array`
- **GetLexemes**() -> `Array`
- **GetSearchResults**(`maxCandidatesToExplore: int`) -> `Instances`
- **HasMoreResults**() -> `bool`
- **InstancePassesFilter**(`instance: Instance`) -> `bool`
- **SetFilter**(`search: string`) -> `null`
