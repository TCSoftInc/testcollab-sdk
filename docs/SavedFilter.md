
# SavedFilter


## Properties

Name | Type
------------ | -------------
`id` | number
`project` | number
`entity` | string
`title` | string
`scope` | string
`filterQuery` | string
`createdBy` | [UserMinified](UserMinified.md)
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { SavedFilter } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "project": 1,
  "entity": TestCase,
  "title": My filter,
  "scope": Public,
  "filterQuery": [],
  "createdBy": null,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "updatedAt": 2019-04-30T17:11:24.000Z,
} satisfies SavedFilter

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SavedFilter
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


