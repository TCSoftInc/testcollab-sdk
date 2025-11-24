
# Filter


## Properties

Name | Type
------------ | -------------
`id` | number
`title` | string
`scope` | string
`filterQuery` | [Array&lt;FilterQuery&gt;](FilterQuery.md)

## Example

```typescript
import type { Filter } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "title": High priority cases,
  "scope": Private,
  "filterQuery": null,
} satisfies Filter

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Filter
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


