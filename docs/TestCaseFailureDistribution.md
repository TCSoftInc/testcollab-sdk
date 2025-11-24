
# TestCaseFailureDistribution


## Properties

Name | Type
------------ | -------------
`casesFrequency` | Array&lt;number&gt;
`labels` | Array&lt;string&gt;

## Example

```typescript
import type { TestCaseFailureDistribution } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "casesFrequency": [15,2,1],
  "labels": ["0-9%","10-19%","20-29%"],
} satisfies TestCaseFailureDistribution

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCaseFailureDistribution
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


