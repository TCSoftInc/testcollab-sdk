
# WebhookSignedEnvelope

Every outbound POST is application/json with this envelope. The body carries verification fields for Google Apps Script receivers that cannot read request headers. The secret itself is never sent.

## Properties

Name | Type
------------ | -------------
`payload` | string
`timestamp` | number
`secretVersion` | number
`signature` | string

## Example

```typescript
import type { WebhookSignedEnvelope } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "payload": null,
  "timestamp": null,
  "secretVersion": null,
  "signature": null,
} satisfies WebhookSignedEnvelope

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookSignedEnvelope
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


