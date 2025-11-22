
# PaymentIntent


## Properties

Name | Type
------------ | -------------
`amount` | number
`amountCapturable` | number
`amountReceived` | number
`clientSecret` | string
`id` | string
`nextAction` | [PaymentIntentNextAction](PaymentIntentNextAction.md)
`status` | string

## Example

```typescript
import type { PaymentIntent } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "amount": 1500,
  "amountCapturable": 1500,
  "amountReceived": 0,
  "clientSecret": pi_1HEwjjJJWKIHQVNwomnrsYyb_secret_KdLF6t9f31BcNZACxSjRDljU7,
  "id": pi_1HEwjjJJWKIHQVNwomnrsYyb,
  "nextAction": null,
  "status": requires_action,
} satisfies PaymentIntent

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PaymentIntent
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


