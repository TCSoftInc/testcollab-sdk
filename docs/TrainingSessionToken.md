
# TrainingSessionToken


## Properties

Name | Type
------------ | -------------
`tokenRequest` | [TrainingSessionTokenRequest](TrainingSessionTokenRequest.md)
`expiresAt` | Date
`clientId` | string

## Example

```typescript
import type { TrainingSessionToken } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "tokenRequest": null,
  "expiresAt": 2025-11-04T10:23:11Z,
  "clientId": user-53,
} satisfies TrainingSessionToken

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TrainingSessionToken
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


