
# SubscriptionPaymentMethodCard


## Properties

Name | Type
------------ | -------------
`brand` | string
`country` | string
`expMonth` | number
`expYear` | number
`last4` | string

## Example

```typescript
import type { SubscriptionPaymentMethodCard } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "brand": visa,
  "country": US,
  "expMonth": 9,
  "expYear": 2020,
  "last4": 4242,
} satisfies SubscriptionPaymentMethodCard

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SubscriptionPaymentMethodCard
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


