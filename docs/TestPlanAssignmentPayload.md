
# TestPlanAssignmentPayload


## Properties

Name | Type
------------ | -------------
`executor` | string
`assignmentCriteria` | string
`assignmentMethod` | string
`assignment` | [TestPlanAssignmentPayloadAssignment](TestPlanAssignmentPayloadAssignment.md)
`project` | number
`testplan` | number

## Example

```typescript
import type { TestPlanAssignmentPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "executor": team,
  "assignmentCriteria": configuration,
  "assignmentMethod": automatic,
  "assignment": null,
  "project": 1,
  "testplan": 1,
} satisfies TestPlanAssignmentPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanAssignmentPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


