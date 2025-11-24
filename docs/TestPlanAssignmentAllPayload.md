
# TestPlanAssignmentAllPayload


## Properties

Name | Type
------------ | -------------
`project` | number
`user` | number
`testplan` | number

## Example

```typescript
import type { TestPlanAssignmentAllPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "project": 1,
  "user": 1,
  "testplan": 1,
} satisfies TestPlanAssignmentAllPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanAssignmentAllPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


