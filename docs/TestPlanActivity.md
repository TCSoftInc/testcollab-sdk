
# TestPlanActivity


## Properties

Name | Type
------------ | -------------
`description` | string
`activityType` | string
`created` | number

## Example

```typescript
import type { TestPlanActivity } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "description": Test plan created,
  "activityType": neutral,
  "created": 1552491237,
} satisfies TestPlanActivity

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanActivity
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


