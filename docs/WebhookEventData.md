
# WebhookEventData

Exactly the member identified by resource_type is populated. Other members are omitted, not null. Large content/attachments are fetched through the existing resource API; changed_fields still identifies edits to them.

## Properties

Name | Type
------------ | -------------
`testCase` | [WebhookTestCaseSnapshot](WebhookTestCaseSnapshot.md)
`suite` | [WebhookSuiteSnapshot](WebhookSuiteSnapshot.md)
`testPlan` | [WebhookTestPlanSnapshot](WebhookTestPlanSnapshot.md)
`executedTestCase` | [WebhookExecutionSnapshot](WebhookExecutionSnapshot.md)
`testPlanRun` | [WebhookTestPlanRunSnapshot](WebhookTestPlanRunSnapshot.md)

## Example

```typescript
import type { WebhookEventData } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "testCase": null,
  "suite": null,
  "testPlan": null,
  "executedTestCase": null,
  "testPlanRun": null,
} satisfies WebhookEventData

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookEventData
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


