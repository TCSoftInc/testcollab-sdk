
# TestCasesSortOrderPayload


## Properties

Name | Type
------------ | -------------
`testCase` | [TestCaseSortProperty](TestCaseSortProperty.md)
`project` | number

## Example

```typescript
import type { TestCasesSortOrderPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "testCase": null,
  "project": 1,
} satisfies TestCasesSortOrderPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCasesSortOrderPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


