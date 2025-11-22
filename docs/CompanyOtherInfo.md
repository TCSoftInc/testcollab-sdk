
# CompanyOtherInfo


## Properties

Name | Type
------------ | -------------
`country` | string
`countryCode` | string
`role` | string
`companySize` | number
`teamSize` | number
`manages` | string
`phone` | string

## Example

```typescript
import type { CompanyOtherInfo } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "country": United States,
  "countryCode": US,
  "role": Business Owner,
  "companySize": null,
  "teamSize": null,
  "manages": Projects for clients,
  "phone": null,
} satisfies CompanyOtherInfo

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CompanyOtherInfo
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


