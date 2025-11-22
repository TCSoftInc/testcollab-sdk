
# TestCaseRefCollection


## Properties

Name | Type
------------ | -------------
`testCases` | Array&lt;number&gt;
`selector` | [Array&lt;FilterQuery&gt;](FilterQuery.md)

## Example

```typescript
import type { TestCaseRefCollection } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "testCases": [1,2,3],
  "selector": null,
} satisfies TestCaseRefCollection

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCaseRefCollection
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


