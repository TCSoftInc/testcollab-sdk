
# ExternalImportStatus


## Properties

Name | Type
------------ | -------------
`id` | number
`importType` | string
`projectId` | number
`sourceProject` | string
`status` | string
`stage` | string
`progress` | [ExternalImportProgress](ExternalImportProgress.md)
`stats` | [ExternalImportStats](ExternalImportStats.md)
`throttle` | [ExternalImportThrottle](ExternalImportThrottle.md)
`lastActivity` | string
`startedAt` | string
`updatedAt` | string
`completedAt` | string
`error` | string

## Example

```typescript
import type { ExternalImportStatus } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 18,
  "importType": xray,
  "projectId": 42,
  "sourceProject": ABC,
  "status": fetching_cases,
  "stage": Importing test cases,
  "progress": null,
  "stats": null,
  "throttle": null,
  "lastActivity": Created "Login with valid credentials",
  "startedAt": 2026-04-08T14:20:11.000Z,
  "updatedAt": 2026-04-08T14:23:04.000Z,
  "completedAt": 2026-04-08T14:24:23.000Z,
  "error": Authentication failed: invalid client secret,
} satisfies ExternalImportStatus

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExternalImportStatus
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


