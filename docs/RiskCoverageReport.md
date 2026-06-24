
# RiskCoverageReport


## Properties

Name | Type
------------ | -------------
`project` | number
`testplan` | number
`totalRisks` | number
`coveredRisks` | number
`residualRiskBand` | string
`coverageByLevel` | [Array&lt;RiskCoverageLevel&gt;](RiskCoverageLevel.md)
`burndown` | [Array&lt;RiskBurndownItem&gt;](RiskBurndownItem.md)

## Example

```typescript
import type { RiskCoverageReport } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "project": 1,
  "testplan": 42,
  "totalRisks": 14,
  "coveredRisks": 11,
  "residualRiskBand": medium,
  "coverageByLevel": null,
  "burndown": null,
} satisfies RiskCoverageReport

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RiskCoverageReport
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


