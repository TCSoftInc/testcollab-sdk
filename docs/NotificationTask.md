
# NotificationTask


## Properties

Name | Type
------------ | -------------
`task` | string
`status` | number
`percentDone` | number

## Example

```typescript
import type { NotificationTask } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "task": Deleting test cases,
  "status": 1,
  "percentDone": 10,
} satisfies NotificationTask

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as NotificationTask
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


