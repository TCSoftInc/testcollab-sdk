
# SubscriptionSchedulePhase


## Properties

Name | Type
------------ | -------------
`plans` | [Array&lt;SubscriptionSchedulePhasePlansInner&gt;](SubscriptionSchedulePhasePlansInner.md)
`endDate` | string
`startDate` | string

## Example

```typescript
import type { SubscriptionSchedulePhase } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "plans": null,
  "endDate": 1588913473,
  "startDate": 1588593473,
} satisfies SubscriptionSchedulePhase

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SubscriptionSchedulePhase
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


