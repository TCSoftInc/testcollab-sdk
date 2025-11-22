
# BulkUpdateTestplanCasesPayload


## Properties

Name | Type
------------ | -------------
`actionType` | string
`testcases` | Array&lt;number&gt;
`project` | number
`testplan` | number
`testPlanConfig` | number
`regression` | number
`comment` | string
`attachments` | Array&lt;string&gt;
`status` | string
`timeTaken` | number
`assignedTo` | number

## Example

```typescript
import type { BulkUpdateTestplanCasesPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "actionType": null,
  "testcases": null,
  "project": 1,
  "testplan": 1,
  "testPlanConfig": 1,
  "regression": 1,
  "comment": My comment,
  "attachments": null,
  "status": passed,
  "timeTaken": 1,
  "assignedTo": 1,
} satisfies BulkUpdateTestplanCasesPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BulkUpdateTestplanCasesPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


