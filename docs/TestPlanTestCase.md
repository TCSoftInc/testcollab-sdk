
# TestPlanTestCase


## Properties

Name | Type
------------ | -------------
`id` | number
`testCase` | [TestCaseMinified](TestCaseMinified.md)
`status` | string
`timeTaken` | number
`avgTimePerExec` | number
`results` | [Array&lt;ConfigWiseResult&gt;](ConfigWiseResult.md)
`configAssignees` | [Array&lt;ConfigWiseAssignee&gt;](ConfigWiseAssignee.md)
`lastRun` | Date
`assignedTo` | [UserMinified](UserMinified.md)
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { TestPlanTestCase } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "testCase": null,
  "status": unexecuted,
  "timeTaken": 120,
  "avgTimePerExec": 100,
  "results": null,
  "configAssignees": null,
  "lastRun": 2019-06-10T09:12:33.001Z,
  "assignedTo": null,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "updatedAt": 2019-04-30T17:11:24.000Z,
} satisfies TestPlanTestCase

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanTestCase
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


