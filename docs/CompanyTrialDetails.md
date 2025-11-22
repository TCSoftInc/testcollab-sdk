
# CompanyTrialDetails


## Properties

Name | Type
------------ | -------------
`isActive` | boolean
`expiration` | number
`extendedTrial` | boolean
`plan` | string

## Example

```typescript
import type { CompanyTrialDetails } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "isActive": true,
  "expiration": 1583193600,
  "extendedTrial": false,
  "plan": null,
} satisfies CompanyTrialDetails

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CompanyTrialDetails
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


