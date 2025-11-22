
# ExecutedTestCasePayload


## Properties

Name | Type
------------ | -------------
`id` | number
`testPlanTestCase` | number
`testCaseRevision` | number
`project` | number
`testPlan` | number
`testPlanConfig` | number
`assignedTo` | number
`regression` | number
`comment` | string
`attachments` | Array&lt;string&gt;
`status` | string
`timeTaken` | number
`stepWiseResult` | [Array&lt;StepWiseResult&gt;](StepWiseResult.md)
`testdatasetWiseResult` | [Array&lt;TestDatasetWiseResult&gt;](TestDatasetWiseResult.md)

## Example

```typescript
import type { ExecutedTestCasePayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "testPlanTestCase": 1,
  "testCaseRevision": 1,
  "project": 1,
  "testPlan": 1,
  "testPlanConfig": 1,
  "assignedTo": 1,
  "regression": 1,
  "comment": My comment,
  "attachments": null,
  "status": passed,
  "timeTaken": 1,
  "stepWiseResult": null,
  "testdatasetWiseResult": null,
} satisfies ExecutedTestCasePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExecutedTestCasePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


