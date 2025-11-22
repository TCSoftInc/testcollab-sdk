
# TestPlan


## Properties

Name | Type
------------ | -------------
`id` | number
`archived` | boolean
`title` | string
`priority` | number
`assignedTo` | [Array&lt;UserMinified&gt;](UserMinified.md)
`status` | number
`results` | [TestPlanResults](.md)
`testPlanFolder` | [TestPlanFolder](.md)
`estimate` | number
`timeSpent` | number
`createdBy` | [UserMinified](.md)
`actualStartDate` | string
`startDate` | string
`endDate` | string
`createdAt` | string
`updatedAt` | string
`lastRun` | string
`description` | string
`customFields` | [Array&lt;CustomFieldCollectionOutput&gt;](CustomFieldCollectionOutput.md)
`isPublic` | number

## Example

```typescript
import type { TestPlan } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "archived": false,
  "title": My first test plan,
  "priority": 1,
  "assignedTo": null,
  "status": 1,
  "results": null,
  "testPlanFolder": null,
  "estimate": 1200,
  "timeSpent": 1200,
  "createdBy": null,
  "actualStartDate": 2019-04-30T17:11:24.000Z,
  "startDate": 2019-04-30T17:11:24.000Z,
  "endDate": 2019-09-30T17:11:24.000Z,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "updatedAt": 2019-04-30T17:11:24.000Z,
  "lastRun": 2019-05-30T17:11:24.000Z,
  "description": test plan description,
  "customFields": null,
  "isPublic": null,
} satisfies TestPlan

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlan
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


