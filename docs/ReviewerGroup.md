
# ReviewerGroup


## Properties

Name | Type
------------ | -------------
`id` | number
`project` | number
`name` | string
`members` | Array&lt;number&gt;
`deletedAt` | string
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { ReviewerGroup } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "project": 1,
  "name": L1 reviewers,
  "members": [11,12],
  "deletedAt": null,
  "createdAt": 2026-10-23T05:00:00.000Z,
  "updatedAt": 2026-10-23T05:00:00.000Z,
} satisfies ReviewerGroup

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReviewerGroup
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


