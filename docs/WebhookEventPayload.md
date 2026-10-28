
# WebhookEventPayload

Immutable event delivered to the receiver. Business events require resource_type/resource_id/resource_version. A synthetic webhook.test omits real resource identifiers. Status events include previous_data and data with native numeric plan/run statuses or string execution statuses.

## Properties

Name | Type
------------ | -------------
`schemaVersion` | string
`eventId` | string
`eventType` | [WebhookEventType](WebhookEventType.md)
`occurredAt` | string
`project` | number
`resourceType` | [WebhookResourceType](WebhookResourceType.md)
`resourceId` | number
`resourceVersion` | number
`correlationId` | string
`changedFields` | Set&lt;string&gt;
`cause` | [WebhookEventCause](WebhookEventCause.md)
`previousData` | [WebhookEventData](WebhookEventData.md)
`data` | [WebhookEventData](WebhookEventData.md)

## Example

```typescript
import type { WebhookEventPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "schemaVersion": null,
  "eventId": null,
  "eventType": null,
  "occurredAt": 2026-10-23T12:00:00.000Z,
  "project": null,
  "resourceType": null,
  "resourceId": null,
  "resourceVersion": null,
  "correlationId": null,
  "changedFields": null,
  "cause": null,
  "previousData": null,
  "data": null,
} satisfies WebhookEventPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookEventPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


