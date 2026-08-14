
# RequirementLinkSync


## Properties

Name | Type
------------ | -------------
`id` | number
`desiredState` | string
`syncStatus` | string
`attempts` | number
`lastError` | string
`lastSyncedAt` | string
`nextRetryAt` | string

## Example

```typescript
import type { RequirementLinkSync } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 42,
  "desiredState": null,
  "syncStatus": null,
  "attempts": 2,
  "lastError": null,
  "lastSyncedAt": 2026-08-13T12:00:00.000Z,
  "nextRetryAt": 2026-08-13T12:05:00.000Z,
} satisfies RequirementLinkSync

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RequirementLinkSync
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


