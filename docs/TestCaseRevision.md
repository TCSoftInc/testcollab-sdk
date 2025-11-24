
# TestCaseRevision


## Properties

Name | Type
------------ | -------------
`id` | number
`revision` | number
`modifiedFields` | [TestCaseRevisionModifiedFields](TestCaseRevisionModifiedFields.md)
`testcase` | number
`isHead` | boolean
`createdAt` | string
`updatedAt` | string
`updatedBy` | number
`actionType` | string
`title` | string
`suite` | [Suite](Suite.md)
`description` | string
`steps` | [Array&lt;Step&gt;](Step.md)
`stepsParsed` | [Array&lt;StepParsed&gt;](StepParsed.md)
`priority` | number
`tags` | [Array&lt;Tag&gt;](Tag.md)
`requirements` | [Array&lt;Requirement&gt;](Requirement.md)
`attachments` | [Array&lt;Upload&gt;](Upload.md)
`customFields` | [Array&lt;CustomFieldCollectionOutput&gt;](CustomFieldCollectionOutput.md)
`sortOrder` | number
`testcaseCreatedAt` | string
`testcaseUpdatedAt` | string
`createdBy` | [UserMinified](UserMinified.md)
`lastRunStatus` | string
`runCount` | number
`avgExecutionTime` | number
`lastRunOn` | string
`failureRate` | number
`isReference` | boolean
`sourceId` | number
`sourceProject` | number
`reviewComments` | string
`reviewer` | number
`poster` | number
`reviewStatus` | number
`automationStatus` | number
`automationInfo` | string

## Example

```typescript
import type { TestCaseRevision } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "revision": 1,
  "modifiedFields": null,
  "testcase": 1,
  "isHead": false,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "updatedAt": 2019-04-30T17:11:24.000Z,
  "updatedBy": 1,
  "actionType": create,
  "title": Test case 1,
  "suite": null,
  "description": This is my test case,
  "steps": null,
  "stepsParsed": null,
  "priority": 1,
  "tags": null,
  "requirements": null,
  "attachments": null,
  "customFields": null,
  "sortOrder": 1,
  "testcaseCreatedAt": 2019-07-21T14:50:55.000Z,
  "testcaseUpdatedAt": 2019-08-21T14:50:55.000Z,
  "createdBy": null,
  "lastRunStatus": passed,
  "runCount": 1,
  "avgExecutionTime": 10,
  "lastRunOn": 2019-10-21T14:50:55.000Z,
  "failureRate": 0,
  "isReference": false,
  "sourceId": 1,
  "sourceProject": 1,
  "reviewComments": null,
  "reviewer": null,
  "poster": null,
  "reviewStatus": null,
  "automationStatus": null,
  "automationInfo": null,
} satisfies TestCaseRevision

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCaseRevision
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


