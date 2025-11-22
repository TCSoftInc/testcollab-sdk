
# InvoiceProrationItems


## Properties

Name | Type
------------ | -------------
`id` | string
`amount` | string
`currency` | string
`description` | string
`period` | [InvoiceProrationItemsPeriod](InvoiceProrationItemsPeriod.md)
`total` | number
`plan` | [SubscriptionPlan](SubscriptionPlan.md)

## Example

```typescript
import type { InvoiceProrationItems } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": il_dfkjr9ur3,
  "amount": -43986,
  "currency": usd,
  "description": Unused time on Premium after 08 May 2020,
  "period": null,
  "total": 1500,
  "plan": null,
} satisfies InvoiceProrationItems

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as InvoiceProrationItems
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


