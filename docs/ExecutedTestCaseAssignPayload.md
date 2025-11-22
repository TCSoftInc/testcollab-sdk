
# ExecutedTestCaseAssignPayload


## Properties

Name | Type
------------ | -------------
`testPlanTestCase` | number
`testPlanConfig` | number
`assignedTo` | number
`testPlan` | number

## Example

```typescript
import type { ExecutedTestCaseAssignPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "testPlanTestCase": null,
  "testPlanConfig": null,
  "assignedTo": null,
  "testPlan": null,
} satisfies ExecutedTestCaseAssignPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExecutedTestCaseAssignPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


