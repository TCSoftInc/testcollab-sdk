
# InvitationPayload


## Properties

Name | Type
------------ | -------------
`id` | number
`email` | string
`company` | number
`role` | number
`projects` | Array&lt;number&gt;

## Example

```typescript
import type { InvitationPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "email": abhi@testcollab.io,
  "company": 1,
  "role": 1,
  "projects": [1,2,4],
} satisfies InvitationPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as InvitationPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


