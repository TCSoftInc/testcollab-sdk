
# WebhookTestCaseSnapshot


## Properties

Name | Type
------------ | -------------
`id` | number
`title` | string
`customFields` | [Array&lt;WebhookCustomFieldValue&gt;](WebhookCustomFieldValue.md)
`displayNumber` | number
`suite` | number
`priority` | number
`archived` | boolean
`trashEntry` | number

## Example

```typescript
import type { WebhookTestCaseSnapshot } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "title": null,
  "customFields": null,
  "displayNumber": null,
  "suite": null,
  "priority": null,
  "archived": null,
  "trashEntry": null,
} satisfies WebhookTestCaseSnapshot

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookTestCaseSnapshot
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


