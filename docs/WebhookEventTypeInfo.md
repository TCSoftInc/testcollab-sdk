
# WebhookEventTypeInfo


## Properties

Name | Type
------------ | -------------
`name` | [WebhookBusinessEventType](WebhookBusinessEventType.md)
`description` | string
`resourceType` | [WebhookResourceType](WebhookResourceType.md)

## Example

```typescript
import type { WebhookEventTypeInfo } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": null,
  "description": null,
  "resourceType": null,
} satisfies WebhookEventTypeInfo

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookEventTypeInfo
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


