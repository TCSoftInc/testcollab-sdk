
# WebhookEventCause


## Properties

Name | Type
------------ | -------------
`action` | string
`rootResourceType` | [WebhookResourceType](WebhookResourceType.md)
`rootResourceId` | number

## Example

```typescript
import type { WebhookEventCause } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "action": null,
  "rootResourceType": null,
  "rootResourceId": null,
} satisfies WebhookEventCause

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookEventCause
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


