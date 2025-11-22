
# UserEditPayload


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`aboutMe` | string
`email` | string
`password` | string
`currentPassword` | string
`avatar` | string

## Example

```typescript
import type { UserEditPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "name": Shriti Grover,
  "aboutMe": I am a tester,
  "email": shriti@testcollab.com,
  "password": password,
  "currentPassword": password,
  "avatar": filehash123,
} satisfies UserEditPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UserEditPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


