
# WebhookDelivery

One delivery of an event to an endpoint. event is the management API\'s event record ID; event_id is the stable UUID receivers use to deduplicate retries. The project is in the query.

## Properties

Name | Type
------------ | -------------
`id` | number
`webhook` | number
`event` | number
`eventId` | string
`eventType` | [WebhookEventType](WebhookEventType.md)
`status` | [WebhookDeliveryState](WebhookDeliveryState.md)
`attemptCount` | number
`maxAttempts` | number
`nextAttemptAt` | string
`createdAt` | string
`attempts` | [Array&lt;WebhookDeliveryAttempt&gt;](WebhookDeliveryAttempt.md)

## Example

```typescript
import type { WebhookDelivery } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "webhook": null,
  "event": null,
  "eventId": null,
  "eventType": null,
  "status": null,
  "attemptCount": null,
  "maxAttempts": null,
  "nextAttemptAt": null,
  "createdAt": null,
  "attempts": null,
} satisfies WebhookDelivery

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookDelivery
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


