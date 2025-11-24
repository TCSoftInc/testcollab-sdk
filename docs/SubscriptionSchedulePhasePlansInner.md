
# SubscriptionSchedulePhasePlansInner


## Properties

Name | Type
------------ | -------------
`plan` | string
`taxRates` | [Array&lt;TaxRate&gt;](TaxRate.md)

## Example

```typescript
import type { SubscriptionSchedulePhasePlansInner } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "plan": e-m-5,
  "taxRates": null,
} satisfies SubscriptionSchedulePhasePlansInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SubscriptionSchedulePhasePlansInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


