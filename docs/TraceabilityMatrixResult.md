
# TraceabilityMatrixResult


## Properties

Name | Type
------------ | -------------
`requirements` | [Array&lt;RequirementMinified&gt;](RequirementMinified.md)
`testcases` | [Array&lt;TestCaseMinified&gt;](TestCaseMinified.md)
`relationData` | [Array&lt;TraceabilityMatrixRelation&gt;](TraceabilityMatrixRelation.md)
`queue` | [Queue](Queue.md)
`totalRequirement` | number

## Example

```typescript
import type { TraceabilityMatrixResult } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "requirements": null,
  "testcases": null,
  "relationData": null,
  "queue": null,
  "totalRequirement": null,
} satisfies TraceabilityMatrixResult

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TraceabilityMatrixResult
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


