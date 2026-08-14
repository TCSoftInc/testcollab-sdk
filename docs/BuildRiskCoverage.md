
# BuildRiskCoverage

Risk coverage scoped to a build (TCV-6726): a risk is \"covered\" when at least one of its linked test cases was executed (any non-unexecuted status) in a test plan linked to the build. Uses Risk-Based Testing. 

## Properties

Name | Type
------------ | -------------
`totalRisks` | number
`coveredRisks` | number
`uncoveredHighCount` | number
`risks` | [Array&lt;BuildRiskCoverageItem&gt;](BuildRiskCoverageItem.md)

## Example

```typescript
import type { BuildRiskCoverage } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "totalRisks": 13,
  "coveredRisks": 12,
  "uncoveredHighCount": 1,
  "risks": null,
} satisfies BuildRiskCoverage

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BuildRiskCoverage
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


