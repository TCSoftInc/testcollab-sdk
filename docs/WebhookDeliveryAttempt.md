
# WebhookDeliveryAttempt


## Properties

Name | Type
------------ | -------------
`attempt` | number
`secretVersion` | number
`startedAt` | string
`completedAt` | string
`durationMs` | number
`requestUrl` | string
`requestHeaders` | [Array&lt;WebhookHeader&gt;](WebhookHeader.md)
`requestBody` | string
`requestTruncated` | boolean
`responseStatus` | number
`responseHeaders` | [Array&lt;WebhookHeader&gt;](WebhookHeader.md)
`responseBody` | string
`responseTruncated` | boolean
`errorKind` | string
`error` | string

## Example

```typescript
import type { WebhookDeliveryAttempt } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "attempt": null,
  "secretVersion": null,
  "startedAt": null,
  "completedAt": null,
  "durationMs": null,
  "requestUrl": null,
  "requestHeaders": null,
  "requestBody": null,
  "requestTruncated": null,
  "responseStatus": null,
  "responseHeaders": null,
  "responseBody": null,
  "responseTruncated": null,
  "errorKind": null,
  "error": null,
} satisfies WebhookDeliveryAttempt

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookDeliveryAttempt
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


