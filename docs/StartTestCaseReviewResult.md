
# StartTestCaseReviewResult


## Properties

Name | Type
------------ | -------------
`id` | number
`revision` | number
`reviewer` | number
`reviewerGroup` | number

## Example

```typescript
import type { StartTestCaseReviewResult } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 7,
  "revision": 42,
  "reviewer": 11,
  "reviewerGroup": 1,
} satisfies StartTestCaseReviewResult

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as StartTestCaseReviewResult
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


