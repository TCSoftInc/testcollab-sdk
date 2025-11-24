
# SubscriptionInvoice


## Properties

Name | Type
------------ | -------------
`id` | string
`paid` | boolean
`periodStart` | string
`periodEnd` | string
`total` | number
`postPaymentCreditNotesAmount` | string
`prePaymentCreditNotesAmount` | string
`receiptNumber` | string
`startingBalance` | string
`statementDescriptor` | string
`status` | string
`amountDue` | number
`amountPaid` | number
`amountRemaining` | number
`applicationFeeAmount` | string
`attemptCount` | number
`attempted` | boolean
`subtotal` | number
`tax` | number
`taxPercent` | string
`created` | string
`paymentIntent` | [PaymentIntent](PaymentIntent.md)

## Example

```typescript
import type { SubscriptionInvoice } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": in_dfkjr9ur3,
  "paid": true,
  "periodStart": 1561117418,
  "periodEnd": 1563709418,
  "total": 1500,
  "postPaymentCreditNotesAmount": 0,
  "prePaymentCreditNotesAmount": 0,
  "receiptNumber": null,
  "startingBalance": 0,
  "statementDescriptor": null,
  "status": paid,
  "amountDue": 7000,
  "amountPaid": 7000,
  "amountRemaining": 0,
  "applicationFeeAmount": null,
  "attemptCount": 1,
  "attempted": true,
  "subtotal": 89493,
  "tax": null,
  "taxPercent": null,
  "created": 1563709418,
  "paymentIntent": null,
} satisfies SubscriptionInvoice

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SubscriptionInvoice
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


