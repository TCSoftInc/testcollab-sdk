
# ReleaseReadinessTestPlanRun

Minimal info about the latest run (regression) of a test plan within the release. 

## Properties

Name | Type
------------ | -------------
`id` | number
`iteration` | number
`status` | string
`createdAt` | string

## Example

```typescript
import type { ReleaseReadinessTestPlanRun } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 23,
  "iteration": 3,
  "status": 2,
  "createdAt": 2025-02-10T14:30:00.000Z,
} satisfies ReleaseReadinessTestPlanRun

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReleaseReadinessTestPlanRun
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


