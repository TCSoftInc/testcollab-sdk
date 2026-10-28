
# Webhook

Shared create/update/response model. id is response-only; enabled, timeout_seconds and max_attempts use the documented defaults when omitted from a request and are always returned. The project comes from the required query parameter. All endpoints share that project\'s single signing secret; no secret is accepted or returned here.

## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`url` | string
`events` | [Set&lt;WebhookBusinessEventType&gt;](WebhookBusinessEventType.md)
`enabled` | boolean
`timeoutSeconds` | number
`maxAttempts` | number

## Example

```typescript
import type { Webhook } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "name": null,
  "url": null,
  "events": null,
  "enabled": null,
  "timeoutSeconds": null,
  "maxAttempts": null,
} satisfies Webhook

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Webhook
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


