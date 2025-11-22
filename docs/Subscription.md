
# Subscription


## Properties

Name | Type
------------ | -------------
`id` | string
`collectionMethod` | string
`created` | string
`currentPeriodEnd` | string
`currentPeriodStart` | string
`cancelAtPeriodEnd` | boolean
`daysUntilDue` | number
`discount` | number
`plan` | [SubscriptionPlan](SubscriptionPlan.md)
`customer` | [StripeCustomer](StripeCustomer.md)
`status` | string
`taxPercent` | number
`defaultPaymentMethod` | [SubscriptionPaymentMethod](SubscriptionPaymentMethod.md)
`latestInvoice` | [SubscriptionInvoice](SubscriptionInvoice.md)
`items` | [SubscriptionItems](SubscriptionItems.md)
`defaultTaxRates` | [Array&lt;SubscriptionTaxRate&gt;](SubscriptionTaxRate.md)

## Example

```typescript
import type { Subscription } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": sub_i89j4f94jf94,
  "collectionMethod": charge_automatically,
  "created": 1588593473,
  "currentPeriodEnd": 1591271873,
  "currentPeriodStart": 1588593473,
  "cancelAtPeriodEnd": false,
  "daysUntilDue": null,
  "discount": null,
  "plan": null,
  "customer": null,
  "status": active,
  "taxPercent": null,
  "defaultPaymentMethod": null,
  "latestInvoice": null,
  "items": null,
  "defaultTaxRates": null,
} satisfies Subscription

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Subscription
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


