
# LoggedInUserUser


## Properties

Name | Type
------------ | -------------
`id` | string
`username` | string
`email` | string
`role` | [RoleMini](RoleMini.md)

## Example

```typescript
import type { LoggedInUserUser } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "username": root,
  "email": abhi@testcollab.com,
  "role": null,
} satisfies LoggedInUserUser

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as LoggedInUserUser
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


