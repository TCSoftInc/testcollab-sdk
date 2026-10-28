
# WebhookCopyPayload

Copies the selected endpoints in one transaction. Either all copies are saved or none.

## Properties

Name | Type
------------ | -------------
`sourceProject` | number
`webhooks` | [Array&lt;WebhookCopyItem&gt;](WebhookCopyItem.md)

## Example

```typescript
import type { WebhookCopyPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "sourceProject": null,
  "webhooks": null,
} satisfies WebhookCopyPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookCopyPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


