
# SaasInstance


## Properties

Name | Type
------------ | -------------
`companyName` | string
`plan` | string
`planStatus` | string
`billingEmail` | string
`trialDetails` | [SaasInstanceTrialDetails](SaasInstanceTrialDetails.md)
`usageDetails` | [SaasInstanceUsageDetails](SaasInstanceUsageDetails.md)
`address` | string
`city` | string
`state` | string
`country` | string

## Example

```typescript
import type { SaasInstance } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "companyName": Test Collab Software Inc.,
  "plan": premium,
  "planStatus": trial,
  "billingEmail": info@giga.com,
  "trialDetails": null,
  "usageDetails": null,
  "address": 21 Jump st.,
  "city": Fredericton,
  "state": NB,
  "country": Canada,
} satisfies SaasInstance

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SaasInstance
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


