
# StripeCustomer


## Properties

Name | Type
------------ | -------------
`id` | string
`address` | [SubscriptionBillingDetails](SubscriptionBillingDetails.md)
`created` | string
`email` | string
`name` | string
`invoiceSettings` | [StripeCustomerInvoiceSettings](StripeCustomerInvoiceSettings.md)
`phone` | string

## Example

```typescript
import type { StripeCustomer } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": cus_i89j4f94jf94,
  "address": null,
  "created": 1588593473,
  "email": contact@gigapromoters.com,
  "name": My company,
  "invoiceSettings": null,
  "phone": null,
} satisfies StripeCustomer

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as StripeCustomer
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


