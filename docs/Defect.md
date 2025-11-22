
# Defect


## Properties

Name | Type
------------ | -------------
`id` | number
`project` | number
`externalId` | string
`title` | string
`userComment` | string
`defectUrl` | string
`defectStatus` | string
`testcase` | [TestCase](TestCase.md)
`testplan` | [TestPlanMinified](TestPlanMinified.md)
`testcaserevision` | [TestCaseRevision](TestCaseRevision.md)
`createdBy` | [User](User.md)
`updatedBy` | [User](User.md)
`createdAt` | string
`updatedAt` | string
`testplantestcase` | [TestPlanTestCaseMinified](TestPlanTestCaseMinified.md)
`stepNumber` | number
`status` | number
`description` | string
`executedtestcase` | number
`defectConfig` | string
`issueManager` | string

## Example

```typescript
import type { Defect } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "project": 1,
  "externalId": ISSUE-1,
  "title": Test case failed - auth check,
  "userComment": Failed due to wrong password,
  "defectUrl": null,
  "defectStatus": null,
  "testcase": null,
  "testplan": null,
  "testcaserevision": null,
  "createdBy": null,
  "updatedBy": null,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "updatedAt": 2019-04-30T17:11:24.000Z,
  "testplantestcase": null,
  "stepNumber": null,
  "status": 1,
  "description": null,
  "executedtestcase": 1,
  "defectConfig": null,
  "issueManager": null,
} satisfies Defect

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Defect
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


