
# CustomerSubscriptionsInfo


## Properties

Name | Type
------------ | -------------
`subscriptions` | [Array&lt;Subscription&gt;](Subscription.md)
`schedule` | [SubscriptionSchedule](SubscriptionSchedule.md)
`fastspringSchedule` | string
`trial` | boolean

## Example

```typescript
import type { CustomerSubscriptionsInfo } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "subscriptions": null,
  "schedule": null,
  "fastspringSchedule": null,
  "trial": false,
} satisfies CustomerSubscriptionsInfo

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CustomerSubscriptionsInfo
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


