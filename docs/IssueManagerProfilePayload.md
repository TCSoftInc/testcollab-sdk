
# IssueManagerProfilePayload


## Properties

Name | Type
------------ | -------------
`name` | string
`issueManager` | string
`_configuration` | string

## Example

```typescript
import type { IssueManagerProfilePayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": Main bug tracker,
  "issueManager": JIRA,
  "_configuration": {},
} satisfies IssueManagerProfilePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as IssueManagerProfilePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


