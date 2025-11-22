
# TestPlanResults


## Properties

Name | Type
------------ | -------------
`overall` | [ResultSummary](.md)
`configWise` | [Array&lt;TestPlanResultsConfigWiseInner&gt;](TestPlanResultsConfigWiseInner.md)

## Example

```typescript
import type { TestPlanResults } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "overall": null,
  "configWise": null,
} satisfies TestPlanResults

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanResults
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


