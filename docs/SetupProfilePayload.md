
# SetupProfilePayload


## Properties

Name | Type
------------ | -------------
`name` | string
`inviteCode` | string
`password` | string

## Example

```typescript
import type { SetupProfilePayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "name": Shriti Grover,
  "inviteCode": abc123,
  "password": password,
} satisfies SetupProfilePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SetupProfilePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


