
# WebhookCopyItem

The copy keeps the source name, events and enabled state. The signing secret is never copied; the copy uses the target project\'s shared secret.

## Properties

Name | Type
------------ | -------------
`id` | number
`url` | string
`timeoutSeconds` | number
`maxAttempts` | number

## Example

```typescript
import type { WebhookCopyItem } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "url": null,
  "timeoutSeconds": null,
  "maxAttempts": null,
} satisfies WebhookCopyItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookCopyItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


