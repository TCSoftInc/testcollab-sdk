
# WebhookTestPlanSnapshot


## Properties

Name | Type
------------ | -------------
`id` | number
`title` | string
`customFields` | [Array&lt;WebhookCustomFieldValue&gt;](WebhookCustomFieldValue.md)
`displayNumber` | number
`testPlanFolder` | number
`startDate` | string
`endDate` | string
`archived` | boolean
`status` | number
`statusLabel` | string
`progress` | string
`results` | [TestPlanResults](TestPlanResults.md)

## Example

```typescript
import type { WebhookTestPlanSnapshot } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "title": null,
  "customFields": null,
  "displayNumber": null,
  "testPlanFolder": null,
  "startDate": null,
  "endDate": null,
  "archived": null,
  "status": null,
  "statusLabel": null,
  "progress": null,
  "results": null,
} satisfies WebhookTestPlanSnapshot

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookTestPlanSnapshot
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


