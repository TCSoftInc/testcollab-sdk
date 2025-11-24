
# StripeInvoice


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
`subscriptionProrationDate` | string
`subtotal` | number
`tax` | number
`taxPercent` | string
`created` | string

## Example

```typescript
import type { StripeInvoice } from '@testcollab/sdk'

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
  "status": draft,
  "subscriptionProrationDate": 1588902209 (Unix timestamp),
  "subtotal": 89493,
  "tax": null,
  "taxPercent": null,
  "created": 1563709418,
} satisfies StripeInvoice

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as StripeInvoice
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


