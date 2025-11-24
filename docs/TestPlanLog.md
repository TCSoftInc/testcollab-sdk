
# TestPlanLog


## Properties

Name | Type
------------ | -------------
`log` | string
`testPlan` | number
`testPlanTitle` | string
`testCaseTitle` | string
`testPlanConfiguration` | number
`testPlanTestCase` | number
`attachments` | [Array&lt;Upload&gt;](Upload.md)
`project` | [ProjectMini](ProjectMini.md)
`activityType` | string
`user` | [User](User.md)
`createdAt` | string

## Example

```typescript
import type { TestPlanLog } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "log": Test Case assigned to someone,
  "testPlan": 1,
  "testPlanTitle": One test plan,
  "testCaseTitle": One test case,
  "testPlanConfiguration": 1,
  "testPlanTestCase": 1,
  "attachments": null,
  "project": null,
  "activityType": add,
  "user": null,
  "createdAt": 2019-04-30T17:11:24.000Z,
} satisfies TestPlanLog

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanLog
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


