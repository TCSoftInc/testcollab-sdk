
# Invoice


## Properties

Name | Type
------------ | -------------
`id` | string
`number` | string
`paid` | boolean
`periodStart` | string
`periodEnd` | string
`total` | number
`hostedInvoiceUrl` | string
`invoicePdf` | string
`created` | string

## Example

```typescript
import type { Invoice } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "number": 2372647-0006,
  "paid": true,
  "periodStart": 1561117418,
  "periodEnd": 1563709418,
  "total": 1500,
  "hostedInvoiceUrl": https://pay.stripe.com/invoice/invst_n8QssN6rXPwkfK9NNP8BHHeJq0,
  "invoicePdf": https://pay.stripe.com/invoice/invst_n8QssN6rXPwkfK9NNP8BHHeJq0/pdf,
  "created": 1563709418,
} satisfies Invoice

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Invoice
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


