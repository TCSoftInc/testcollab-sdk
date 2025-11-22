
# StripeCustomerInvoiceSettings


## Properties

Name | Type
------------ | -------------
`defaultPaymentMethod` | [SubscriptionPaymentMethod](SubscriptionPaymentMethod.md)

## Example

```typescript
import type { StripeCustomerInvoiceSettings } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "defaultPaymentMethod": null,
} satisfies StripeCustomerInvoiceSettings

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as StripeCustomerInvoiceSettings
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


