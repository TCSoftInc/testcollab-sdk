
# SubscriptionSchedule


## Properties

Name | Type
------------ | -------------
`id` | string
`status` | string
`created` | string
`phases` | [Array&lt;SubscriptionSchedulePhase&gt;](SubscriptionSchedulePhase.md)

## Example

```typescript
import type { SubscriptionSchedule } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": sch_i89j4f94jf94,
  "status": not_started,
  "created": 1588593473,
  "phases": null,
} satisfies SubscriptionSchedule

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SubscriptionSchedule
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


