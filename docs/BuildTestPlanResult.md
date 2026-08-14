
# BuildTestPlanResult

A test plan linked to a build, with its cached result distribution (TCV-6726).

## Properties

Name | Type
------------ | -------------
`id` | number
`displayNumber` | number
`title` | string
`status` | string
`totalCases` | number
`lastRun` | string
`linkedOnly` | boolean
`results` | [BuildTestPlanResultResults](BuildTestPlanResultResults.md)

## Example

```typescript
import type { BuildTestPlanResult } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 12,
  "displayNumber": 12,
  "title": Q2 Regression · Payments core,
  "status": 2,
  "totalCases": 96,
  "lastRun": 2026-06-26,
  "linkedOnly": false,
  "results": null,
} satisfies BuildTestPlanResult

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BuildTestPlanResult
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


