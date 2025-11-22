
# Execution


## Properties

Name | Type
------------ | -------------
`id` | number
`title` | string
`status` | number
`createdBy` | [User](User.md)
`milestone` | [Milestone](Milestone.md)
`startDate` | number
`dueDate` | number
`created` | number
`usersResponsible` | [Array&lt;User&gt;](User.md)
`testCaseStatus` | [Array&lt;ExecutionTestCaseStatusInner&gt;](ExecutionTestCaseStatusInner.md)
`totalTestCases` | number
`customFields` | [Array&lt;CustomFieldCollectionOutput&gt;](CustomFieldCollectionOutput.md)

## Example

```typescript
import type { Execution } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "title": My first execution,
  "status": 1,
  "createdBy": null,
  "milestone": null,
  "startDate": 1552491237,
  "dueDate": 1577836800,
  "created": 1552491237,
  "usersResponsible": null,
  "testCaseStatus": [{"status":"Passed","count":22,"color":"009026"},{"status":"Failed","count":5,"color":"dc2c2e"},{"status":"Skipped","count":3,"color":"ffa432"},{"status":"Unexecuted","count":2,"color":989898}],
  "totalTestCases": 32,
  "customFields": null,
} satisfies Execution

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Execution
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


