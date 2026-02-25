
# ReleaseReadinessRequirementSummary

Summary statistics for requirement coverage within the release. 

## Properties

Name | Type
------------ | -------------
`total` | number
`fullyCovered` | number
`partiallyCovered` | number
`notCovered` | number
`coverageRate` | number

## Example

```typescript
import type { ReleaseReadinessRequirementSummary } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "total": 20,
  "fullyCovered": 12,
  "partiallyCovered": 5,
  "notCovered": 3,
  "coverageRate": 60,
} satisfies ReleaseReadinessRequirementSummary

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReleaseReadinessRequirementSummary
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


