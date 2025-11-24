
# SavedFilterPayload


## Properties

Name | Type
------------ | -------------
`id` | number
`project` | number
`entity` | string
`scope` | string
`title` | string
`filterQuery` | string

## Example

```typescript
import type { SavedFilterPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "project": 1,
  "entity": TestCase,
  "scope": Public,
  "title": My filter,
  "filterQuery": [],
} satisfies SavedFilterPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SavedFilterPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


