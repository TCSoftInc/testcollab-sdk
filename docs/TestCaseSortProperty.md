
# TestCaseSortProperty


## Properties

Name | Type
------------ | -------------
`id` | Array&lt;number&gt;
`suiteId` | number
`oldPosition` | number
`newPosition` | number
`limit` | number

## Example

```typescript
import type { TestCaseSortProperty } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": [1,2,3],
  "suiteId": 1,
  "oldPosition": 1,
  "newPosition": 2,
  "limit": 10,
} satisfies TestCaseSortProperty

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCaseSortProperty
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


