
# UserCreatePayload


## Properties

Name | Type
------------ | -------------
`username` | string
`email` | string
`password` | string

## Example

```typescript
import type { UserCreatePayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "username": myuser,
  "email": abhi@testcollab.com,
  "password": 12345678,
} satisfies UserCreatePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UserCreatePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


