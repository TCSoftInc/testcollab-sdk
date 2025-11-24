
# Invitation


## Properties

Name | Type
------------ | -------------
`id` | number
`email` | string
`company` | [Company](Company.md)
`inviteCode` | string
`projects` | Array&lt;number&gt;
`status` | number
`createdAt` | string

## Example

```typescript
import type { Invitation } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "email": insane.subodh@gmail.com,
  "company": null,
  "inviteCode": Code123,
  "projects": [1,2,4],
  "status": 0,
  "createdAt": 2019-04-30T17:11:24.000Z,
} satisfies Invitation

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Invitation
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


