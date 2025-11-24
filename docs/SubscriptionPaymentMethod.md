
# SubscriptionPaymentMethod


## Properties

Name | Type
------------ | -------------
`id` | string
`card` | [SubscriptionPaymentMethodCard](SubscriptionPaymentMethodCard.md)
`billingDetails` | [SubscriptionPaymentMethodBillingDetails](SubscriptionPaymentMethodBillingDetails.md)
`metadata` | [SubscriptionPaymentMethodMetadata](SubscriptionPaymentMethodMetadata.md)

## Example

```typescript
import type { SubscriptionPaymentMethod } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": pm_1GflU0JJWKIHQVNwAifyiA6v,
  "card": null,
  "billingDetails": null,
  "metadata": null,
} satisfies SubscriptionPaymentMethod

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SubscriptionPaymentMethod
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


