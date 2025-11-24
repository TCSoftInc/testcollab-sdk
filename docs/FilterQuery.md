
# FilterQuery


## Properties

Name | Type
------------ | -------------
`field` | string
`operator` | string
`value` | string

## Example

```typescript
import type { FilterQuery } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "field": title,
  "operator": contains,
  "value": Hello world,
} satisfies FilterQuery

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as FilterQuery
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


