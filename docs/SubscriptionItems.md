
# SubscriptionItems


## Properties

Name | Type
------------ | -------------
`data` | [Array&lt;SubscriptionItemsDataInner&gt;](SubscriptionItemsDataInner.md)
`totalCount` | number

## Example

```typescript
import type { SubscriptionItems } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "data": null,
  "totalCount": 1,
} satisfies SubscriptionItems

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SubscriptionItems
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


