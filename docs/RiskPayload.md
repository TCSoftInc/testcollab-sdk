
# RiskPayload


## Properties

Name | Type
------------ | -------------
`project` | number
`title` | string
`description` | string
`riskType` | number
`status` | number
`likelihood` | number
`impact` | number
`owner` | number
`mitigationStrategy` | string
`residualLikelihood` | number
`residualImpact` | number
`targetDate` | string
`reviewDate` | string
`tags` | Array&lt;number&gt;

## Example

```typescript
import type { RiskPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "project": 1,
  "title": Payment authorization bypass under concurrent sessions,
  "description": null,
  "riskType": 1,
  "status": 1,
  "likelihood": 4,
  "impact": 5,
  "owner": 1,
  "mitigationStrategy": null,
  "residualLikelihood": null,
  "residualImpact": null,
  "targetDate": 2026-07-30T17:11:24.000Z,
  "reviewDate": 2026-07-15T17:11:24.000Z,
  "tags": null,
} satisfies RiskPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RiskPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


