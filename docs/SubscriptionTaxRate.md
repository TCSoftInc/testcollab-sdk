
# SubscriptionTaxRate


## Properties

Name | Type
------------ | -------------
`id` | string
`active` | boolean
`inclusive` | boolean
`displayName` | string
`percentage` | number

## Example

```typescript
import type { SubscriptionTaxRate } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": txr_dfkjr9ur3,
  "active": true,
  "inclusive": true,
  "displayName": Sales Tax,
  "percentage": null,
} satisfies SubscriptionTaxRate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SubscriptionTaxRate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


