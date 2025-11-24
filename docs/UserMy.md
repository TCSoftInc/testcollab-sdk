
# UserMy


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`aboutMe` | string
`email` | string
`avatar` | [Upload](Upload.md)
`username` | string
`lastActive` | Date
`confirmed` | boolean
`rank` | string
`token` | [Token](Token.md)
`projects` | [Array&lt;ProjectUserMinified&gt;](ProjectUserMinified.md)
`companies` | [Array&lt;Company&gt;](Company.md)
`preferences` | [UserPreference](UserPreference.md)
`createdAt` | string
`isGuest` | number
`isCopilot` | number
`intercomHash` | string

## Example

```typescript
import type { UserMy } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "name": Shriti Grover,
  "aboutMe": Short description of user,
  "email": shriti@testcollab.com,
  "avatar": null,
  "username": shritig,
  "lastActive": 2019-06-10T09:12:33.001Z,
  "confirmed": null,
  "rank": null,
  "token": null,
  "projects": null,
  "companies": null,
  "preferences": null,
  "createdAt": 2019-06-10T09:12:33.001Z,
  "isGuest": null,
  "isCopilot": null,
  "intercomHash": null,
} satisfies UserMy

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UserMy
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


