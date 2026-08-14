
# BuildWorkItemTestcase


## Properties

Name | Type
------------ | -------------
`id` | number
`displayNumber` | number
`title` | string
`revision` | number
`executionStatus` | string
`testPlan` | number
`testPlanTitle` | string

## Example

```typescript
import type { BuildWorkItemTestcase } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 81,
  "displayNumber": 301,
  "title": Settlement retry is idempotent,
  "revision": 4,
  "executionStatus": passed,
  "testPlan": 17,
  "testPlanTitle": Payments regression,
} satisfies BuildWorkItemTestcase

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BuildWorkItemTestcase
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


