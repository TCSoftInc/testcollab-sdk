
# TestPlanRegression


## Properties

Name | Type
------------ | -------------
`id` | number
`title` | string
`iteration` | number
`testCaseSelection` | Array&lt;string&gt;
`assignedTo` | [Array&lt;UserMinified&gt;](UserMinified.md)
`status` | number
`result` | [ResultSummary](.md)
`testplan` | number
`timeSpent` | number
`createdBy` | [UserMinified](.md)
`createdAt` | string
`updatedAt` | string
`configurations` | [Array&lt;TestPlanConfiguration&gt;](TestPlanConfiguration.md)
`lastActivity` | string
`pendingQueueId` | number

## Example

```typescript
import type { TestPlanRegression } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "title": Test 1,
  "iteration": 1,
  "testCaseSelection": null,
  "assignedTo": null,
  "status": 1,
  "result": null,
  "testplan": 1,
  "timeSpent": 1200,
  "createdBy": null,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "updatedAt": 2019-04-30T17:11:24.000Z,
  "configurations": null,
  "lastActivity": Test case failed,
  "pendingQueueId": null,
} satisfies TestPlanRegression

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanRegression
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


