
# CompanyOtherInfoPayload


## Properties

Name | Type
------------ | -------------
`company` | number
`otherInfo` | [CompanyOtherInfo](CompanyOtherInfo.md)
`utmCampaign` | string
`isOnboarded` | boolean
`onboardingInfo` | string

## Example

```typescript
import type { CompanyOtherInfoPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "company": 1,
  "otherInfo": null,
  "utmCampaign": null,
  "isOnboarded": true,
  "onboardingInfo": null,
} satisfies CompanyOtherInfoPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CompanyOtherInfoPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


