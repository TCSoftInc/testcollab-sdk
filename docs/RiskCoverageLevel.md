
# RiskCoverageLevel


## Properties

Name | Type
------------ | -------------
`band` | string
`total` | number
`covered` | number
`coveragePct` | number

## Example

```typescript
import type { RiskCoverageLevel } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "band": critical,
  "total": 4,
  "covered": 3,
  "coveragePct": 75,
} satisfies RiskCoverageLevel

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RiskCoverageLevel
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


