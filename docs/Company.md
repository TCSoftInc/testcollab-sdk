
# Company


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`plan` | string
`size` | number
`planStatus` | string
`billingEmail` | string
`trialDetails` | [CompanyTrialDetails](CompanyTrialDetails.md)
`usageDetails` | [CompanyUsageDetails](CompanyUsageDetails.md)
`stripeInfo` | [CompanyStripeInfo](CompanyStripeInfo.md)
`address` | string
`city` | string
`state` | string
`country` | string
`owner` | [User](User.md)
`trialOpted` | boolean
`trialStartedOn` | string
`otherInfo` | [CompanyOtherInfo](CompanyOtherInfo.md)
`createdAt` | string
`stats` | string
`isOnboarded` | boolean
`onboardingInfo` | string

## Example

```typescript
import type { Company } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "name": Test Collab Software Inc.,
  "plan": premium,
  "size": 10,
  "planStatus": trial,
  "billingEmail": info@giga.com,
  "trialDetails": null,
  "usageDetails": null,
  "stripeInfo": null,
  "address": 21 Jump st.,
  "city": Fredericton,
  "state": NB,
  "country": Canada,
  "owner": null,
  "trialOpted": false,
  "trialStartedOn": 2019-04-30T17:11:24.000Z,
  "otherInfo": null,
  "createdAt": 2019-06-10T09:12:33.001Z,
  "stats": null,
  "isOnboarded": false,
  "onboardingInfo": null,
} satisfies Company

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Company
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


