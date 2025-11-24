
# CompanyUsageDetails


## Properties

Name | Type
------------ | -------------
`testCases` | number
`executedCases` | number
`projects` | number
`users` | number

## Example

```typescript
import type { CompanyUsageDetails } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "testCases": 200,
  "executedCases": 200,
  "projects": 5,
  "users": 10,
} satisfies CompanyUsageDetails

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CompanyUsageDetails
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


