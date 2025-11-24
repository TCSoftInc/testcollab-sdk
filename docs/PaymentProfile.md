
# PaymentProfile


## Properties

Name | Type
------------ | -------------
`id` | number
`stripeToken` | string
`users` | number
`billingCycle` | string
`customerId` | string
`stripeSubscriptionId` | string
`subscriptionSchedule` | [SubscriptionSchedule](SubscriptionSchedule.md)
`subscription` | [Subscription](Subscription.md)
`declineCode` | string
`subscriptionCancelled` | boolean
`subscriptionExpiration` | string
`country` | string
`postalCode` | string
`customerTaxId` | string

## Example

```typescript
import type { PaymentProfile } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "stripeToken": dfg566fgh5656,
  "users": 10,
  "billingCycle": yearly,
  "customerId": cus_fiu8jf9u3,
  "stripeSubscriptionId": sub_fiu8jf9u3,
  "subscriptionSchedule": null,
  "subscription": null,
  "declineCode": null,
  "subscriptionCancelled": null,
  "subscriptionExpiration": null,
  "country": CA,
  "postalCode": 85006,
  "customerTaxId": null,
} satisfies PaymentProfile

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PaymentProfile
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


