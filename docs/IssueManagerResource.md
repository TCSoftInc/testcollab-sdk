
# IssueManagerResource


## Properties

Name | Type
------------ | -------------
`project` | number
`name` | string
`resourceList` | [Array&lt;IssueManagerResourceItem&gt;](IssueManagerResourceItem.md)
`resourceInfo` | string

## Example

```typescript
import type { IssueManagerResource } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "project": 1,
  "name": project,
  "resourceList": null,
  "resourceInfo": null,
} satisfies IssueManagerResource

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as IssueManagerResource
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


