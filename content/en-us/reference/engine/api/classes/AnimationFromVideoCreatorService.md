---
title: AnimationFromVideoCreatorService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# AnimationFromVideoCreatorService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **CreateJob**(`filePath: string`) -> `string` [Yields]
- **DownloadJobResult**(`jobId: string`, `outputFilePath: string`) -> `string` [Yields]
- **FullProcess**(`videoFilePath: string`, `progressCallback: Function`) -> `string` [Yields]
- **GetJobStatus**(`jobId: string`) -> `string` [Yields]
