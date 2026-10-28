
# WebhookExecutionSnapshot


## Properties

Name | Type
------------ | -------------
`id` | number
`testCase` | number
`testPlan` | number
`regression` | number
`testPlanConfig` | number
`status` | string
`assignedTo` | number

## Example

```typescript
import type { WebhookExecutionSnapshot } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "testCase": null,
  "testPlan": null,
  "regression": null,
  "testPlanConfig": null,
  "status": null,
  "assignedTo": null,
} satisfies WebhookExecutionSnapshot

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookExecutionSnapshot
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


