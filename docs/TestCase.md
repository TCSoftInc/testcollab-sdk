
# TestCase


## Properties

Name | Type
------------ | -------------
`id` | number
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
`createdAt` | string
`updatedAt` | string
`createdBy` | [UserMinified](UserMinified.md)
`lastRunStatus` | string
`runCount` | number
`avgExecutionTime` | number
`lastRunOn` | string
`failureRate` | number
`isReference` | boolean
`sourceId` | number
`sourceProject` | number
`underReview` | number
`isAutomated` | number
`qacTimeout` | number

## Example

```typescript
import type { TestCase } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
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
  "createdAt": 2019-07-21T14:50:55.000Z,
  "updatedAt": 2019-08-21T14:50:55.000Z,
  "createdBy": null,
  "lastRunStatus": passed,
  "runCount": 1,
  "avgExecutionTime": 10,
  "lastRunOn": 2019-10-21T14:50:55.000Z,
  "failureRate": 0,
  "isReference": false,
  "sourceId": 1,
  "sourceProject": 1,
  "underReview": null,
  "isAutomated": null,
  "qacTimeout": null,
} satisfies TestCase

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCase
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


