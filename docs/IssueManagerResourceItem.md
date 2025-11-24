
# IssueManagerResourceItem


## Properties

Name | Type
------------ | -------------
`id` | number
`key` | string
`name` | string
`extraInfo` | string

## Example

```typescript
import type { IssueManagerResourceItem } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "key": null,
  "name": null,
  "extraInfo": null,
} satisfies IssueManagerResourceItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as IssueManagerResourceItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


