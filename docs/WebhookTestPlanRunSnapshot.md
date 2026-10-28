
# WebhookTestPlanRunSnapshot

Immutable saved run snapshot. Other run details remain available through the existing testplanregressions API. Project appears once in the enclosing event payload.

## Properties

Name | Type
------------ | -------------
`id` | number
`testPlan` | number
`title` | string
`iteration` | number
`status` | number
`build` | number

## Example

```typescript
import type { WebhookTestPlanRunSnapshot } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "testPlan": null,
  "title": null,
  "iteration": null,
  "status": null,
  "build": null,
} satisfies WebhookTestPlanRunSnapshot

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookTestPlanRunSnapshot
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


