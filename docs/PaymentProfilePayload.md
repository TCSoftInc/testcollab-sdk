
# PaymentProfilePayload


## Properties

Name | Type
------------ | -------------
`id` | number
`stripeToken` | string
`users` | number
`billingCycle` | string
`company` | number
`planId` | string
`product` | string
`email` | string
`address` | string
`city` | string
`state` | string
`country` | string
`countryCode` | string
`postalCode` | string
`phone` | string
`name` | string
`trial` | boolean
`customerTaxId` | string
`taxInfo` | [StripeTaxInfo](StripeTaxInfo.md)

## Example

```typescript
import type { PaymentProfilePayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "stripeToken": tok_mastercard,
  "users": 10,
  "billingCycle": yearly,
  "company": 1,
  "planId": p-m-2,
  "product": essential,
  "email": null,
  "address": 21 Jump st.,
  "city": Fredericton,
  "state": NB,
  "country": Canada,
  "countryCode": CA,
  "postalCode": 85006,
  "phone": null,
  "name": null,
  "trial": false,
  "customerTaxId": null,
  "taxInfo": null,
} satisfies PaymentProfilePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PaymentProfilePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


