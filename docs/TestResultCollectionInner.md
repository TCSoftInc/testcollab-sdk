
# TestResultCollectionInner


## Properties

Name | Type
------------ | -------------
`status` | string
`count` | number
`percent` | number

## Example

```typescript
import type { TestResultCollectionInner } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "status": Passed,
  "count": 15,
  "percent": 15,
} satisfies TestResultCollectionInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestResultCollectionInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


