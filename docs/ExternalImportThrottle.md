
# ExternalImportThrottle

Throttle state published by the runner when paused due to rate limits

## Properties

Name | Type
------------ | -------------
`active` | boolean
`service` | string
`message` | string
`resumesAt` | string

## Example

```typescript
import type { ExternalImportThrottle } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "active": false,
  "service": xray-graphql,
  "message": Slowed by Xray rate limits — about 30 seconds remaining,
  "resumesAt": 2026-04-08T14:23:34.000Z,
} satisfies ExternalImportThrottle

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExternalImportThrottle
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


