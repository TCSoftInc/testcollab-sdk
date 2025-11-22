
# SaasInstanceUsageDetails


## Properties

Name | Type
------------ | -------------
`testCases` | number
`executedCases` | number

## Example

```typescript
import type { SaasInstanceUsageDetails } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "testCases": 200,
  "executedCases": 200,
} satisfies SaasInstanceUsageDetails

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SaasInstanceUsageDetails
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


