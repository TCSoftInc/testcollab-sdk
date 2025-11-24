
# IssueManagerLinkPayload


## Properties

Name | Type
------------ | -------------
`authCode` | string
`issueManager` | string
`project` | number
`user` | number
`isDefault` | boolean
`_configuration` | string

## Example

```typescript
import type { IssueManagerLinkPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "authCode": null,
  "issueManager": jira,
  "project": 1,
  "user": 1,
  "isDefault": true,
  "_configuration": {},
} satisfies IssueManagerLinkPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as IssueManagerLinkPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


