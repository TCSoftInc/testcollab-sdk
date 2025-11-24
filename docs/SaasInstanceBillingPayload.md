
# SaasInstanceBillingPayload


## Properties

Name | Type
------------ | -------------
`companyName` | string
`address` | string
`city` | string
`state` | string
`country` | string
`billingEmail` | string
`postalCode` | string

## Example

```typescript
import type { SaasInstanceBillingPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "companyName": Test Collab Software Inc.,
  "address": 21 Jump st.,
  "city": Fredericton,
  "state": NB,
  "country": Canada,
  "billingEmail": info@giga.com,
  "postalCode": 85006,
} satisfies SaasInstanceBillingPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SaasInstanceBillingPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


