
# SubscriptionPlan


## Properties

Name | Type
------------ | -------------
`id` | string
`active` | boolean
`amount` | number
`amountDecimal` | string
`currency` | string
`interval` | string
`intervalCount` | number
`nickname` | string

## Example

```typescript
import type { SubscriptionPlan } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": e-m-2,
  "active": true,
  "amount": 7000,
  "amountDecimal": 7000,
  "currency": usd,
  "interval": month,
  "intervalCount": 1,
  "nickname": Monthly Plan for 2 Users,
} satisfies SubscriptionPlan

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SubscriptionPlan
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


