
# TrainingSessionTokenRequest


## Properties

Name | Type
------------ | -------------
`keyName` | string
`ttl` | number
`capability` | string
`clientId` | string
`timestamp` | number
`nonce` | string
`mac` | string

## Example

```typescript
import type { TrainingSessionTokenRequest } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "keyName": api.key-12345,
  "ttl": 3600000,
  "capability": {"training-session.3201":["subscribe"]},
  "clientId": user-53,
  "timestamp": 1730715791000,
  "nonce": 550e8400-e29b-41d4-a716-446655440000,
  "mac": 4d2a5f9c1c9a4a6a8f3c0d1b2e4f6a7b,
} satisfies TrainingSessionTokenRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TrainingSessionTokenRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


