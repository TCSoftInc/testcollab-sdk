
# PaymentIntentNextAction


## Properties

Name | Type
------------ | -------------
`type` | string
`useStripeSdk` | [PaymentIntentUseStripeSdk](PaymentIntentUseStripeSdk.md)

## Example

```typescript
import type { PaymentIntentNextAction } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "type": use_stripe_sdk,
  "useStripeSdk": null,
} satisfies PaymentIntentNextAction

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PaymentIntentNextAction
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


