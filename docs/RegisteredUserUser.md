
# RegisteredUserUser


## Properties

Name | Type
------------ | -------------
`id` | string
`username` | string
`email` | string

## Example

```typescript
import type { RegisteredUserUser } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "username": root,
  "email": abhi@testcollab.com,
} satisfies RegisteredUserUser

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RegisteredUserUser
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


