
# ProjectMetrics


## Properties

Name | Type
------------ | -------------
`defectCount` | number
`timeTakenInSeconds` | number
`totalCasesCreated` | number
`casesPassed` | [CasesPassed](CasesPassed.md)
`avgTimePerExec` | number
`executionCount` | number

## Example

```typescript
import type { ProjectMetrics } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "defectCount": 2,
  "timeTakenInSeconds": 5,
  "totalCasesCreated": 2,
  "casesPassed": null,
  "avgTimePerExec": 2,
  "executionCount": 2,
} satisfies ProjectMetrics

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProjectMetrics
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


