
# ExecutedTestCase


## Properties

Name | Type
------------ | -------------
`id` | number
`testPlanTestCase` | [TestPlanTestCase](TestPlanTestCase.md)
`testCaseRevision` | [TestCaseRevision](TestCaseRevision.md)
`project` | [Project](Project.md)
`comment` | string
`attachments` | [Array&lt;Upload&gt;](Upload.md)
`testPlanConfig` | number
`testPlan` | number
`regression` | number
`assignedTo` | number
`status` | string
`timeTaken` | number
`executedBy` | [User](User.md)
`stepWiseResult` | [Array&lt;StepWiseResult&gt;](StepWiseResult.md)
`createdAt` | string
`updatedAt` | string
`validationStatus` | number
`validationData` | string
`testdataset` | string
`testdatasetWiseResult` | [Array&lt;TestDatasetWiseResult&gt;](TestDatasetWiseResult.md)
`runOn` | string

## Example

```typescript
import type { ExecutedTestCase } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "testPlanTestCase": null,
  "testCaseRevision": null,
  "project": null,
  "comment": My comment,
  "attachments": null,
  "testPlanConfig": 1,
  "testPlan": 1,
  "regression": 1,
  "assignedTo": 1,
  "status": passed,
  "timeTaken": 1,
  "executedBy": null,
  "stepWiseResult": null,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "updatedAt": 2019-04-30T17:11:24.000Z,
  "validationStatus": null,
  "validationData": null,
  "testdataset": null,
  "testdatasetWiseResult": null,
  "runOn": 2019-04-30T17:11:24.000Z,
} satisfies ExecutedTestCase

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExecutedTestCase
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


