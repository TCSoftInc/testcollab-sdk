
# WebhookBusinessEventType

The 14 subscribable business events, including run creation. executed_test_case.assigned is removed for now (TCV-2175); assignment is sent as the plan\'s assigned_to in test_plan events.

## Properties

Name | Type
------------ | -------------

## Example

```typescript
import type { WebhookBusinessEventType } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
} satisfies WebhookBusinessEventType

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookBusinessEventType
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


