
# WebhookSecret

Shared GET/POST response for the project\'s single signing key. POST returns has_secret=true and the new secret once. No endpoint has its own key.

## Properties

Name | Type
------------ | -------------
`hasSecret` | boolean
`secretVersion` | number
`secret` | string
`generatedAt` | string
`firstGeneratedAt` | string

## Example

```typescript
import type { WebhookSecret } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "hasSecret": null,
  "secretVersion": null,
  "secret": null,
  "generatedAt": null,
  "firstGeneratedAt": null,
} satisfies WebhookSecret

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookSecret
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


