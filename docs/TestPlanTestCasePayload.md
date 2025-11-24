
# TestPlanTestCasePayload


## Properties

Name | Type
------------ | -------------
`testplan` | number
`testcase` | number
`project` | number
`assignedTo` | number
`status` | string
`configAssignees` | [Array&lt;ConfigWiseAssignee&gt;](ConfigWiseAssignee.md)

## Example

```typescript
import type { TestPlanTestCasePayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "testplan": 1,
  "testcase": 1,
  "project": 1,
  "assignedTo": 1,
  "status": unexecuted,
  "configAssignees": null,
} satisfies TestPlanTestCasePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanTestCasePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


