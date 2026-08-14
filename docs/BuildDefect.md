
# BuildDefect

A defect raised against one of the build\'s test plans (TCV-6726).

## Properties

Name | Type
------------ | -------------
`id` | number
`externalId` | string
`title` | string
`status` | string
`defectStatus` | string
`issueManager` | string
`defectUrl` | string
`testPlan` | number
`testPlanTitle` | string
`testcase` | number
`testcaseDisplayNumber` | number

## Example

```typescript
import type { BuildDefect } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 214,
  "externalId": ISS-214,
  "title": Bulk upload rejects file at exactly 10 MB,
  "status": 1,
  "defectStatus": To Do,
  "issueManager": inbuilt,
  "defectUrl": null,
  "testPlan": 12,
  "testPlanTitle": Q2 Regression · Payments core,
  "testcase": 132,
  "testcaseDisplayNumber": 132,
} satisfies BuildDefect

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BuildDefect
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


