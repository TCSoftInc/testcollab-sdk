
# Risk


## Properties

Name | Type
------------ | -------------
`id` | number
`displayNumber` | number
`project` | number
`title` | string
`description` | string
`riskType` | [RiskType](RiskType.md)
`status` | [RiskStatus](RiskStatus.md)
`likelihood` | [RiskScaleValue](RiskScaleValue.md)
`impact` | [RiskScaleValue](RiskScaleValue.md)
`exposure` | number
`exposureBand` | string
`owner` | [User](User.md)
`mitigationStrategy` | string
`residualLikelihood` | [RiskScaleValue](RiskScaleValue.md)
`residualImpact` | [RiskScaleValue](RiskScaleValue.md)
`residualExposure` | number
`targetDate` | string
`reviewDate` | string
`tags` | [Array&lt;Tag&gt;](Tag.md)
`associations` | [Array&lt;RiskAssociation&gt;](RiskAssociation.md)
`verification` | [RiskVerification](RiskVerification.md)
`externalId` | string
`externalUrl` | string
`issueManager` | string
`createdBy` | [User](User.md)
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { Risk } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "displayNumber": 12,
  "project": 1,
  "title": Payment authorization bypass under concurrent sessions,
  "description": null,
  "riskType": null,
  "status": null,
  "likelihood": null,
  "impact": null,
  "exposure": 20,
  "exposureBand": critical,
  "owner": null,
  "mitigationStrategy": null,
  "residualLikelihood": null,
  "residualImpact": null,
  "residualExposure": 8,
  "targetDate": 2026-07-30T17:11:24.000Z,
  "reviewDate": 2026-07-15T17:11:24.000Z,
  "tags": null,
  "associations": null,
  "verification": null,
  "externalId": AB#3402,
  "externalUrl": null,
  "issueManager": null,
  "createdBy": null,
  "createdAt": 2026-04-30T17:11:24.000Z,
  "updatedAt": 2026-04-30T17:11:24.000Z,
} satisfies Risk

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Risk
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


