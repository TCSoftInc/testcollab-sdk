
# SubscriptionBillingDetails


## Properties

Name | Type
------------ | -------------
`city` | string
`country` | string
`line1` | string
`postalCode` | string
`state` | string

## Example

```typescript
import type { SubscriptionBillingDetails } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "city": null,
  "country": null,
  "line1": null,
  "postalCode": 90001,
  "state": null,
} satisfies SubscriptionBillingDetails

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SubscriptionBillingDetails
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


