
# TestCasesProneToErrorResultQuery


## Properties

Name | Type
------------ | -------------
`totalExecs` | number
`casesFailed` | number
`casesFailedPercent` | number
`testCaseTitle` | string
`tcId` | number

## Example

```typescript
import type { TestCasesProneToErrorResultQuery } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "totalExecs": 1,
  "casesFailed": 1,
  "casesFailedPercent": 100,
  "testCaseTitle": Flash messages check,
  "tcId": 26,
} satisfies TestCasesProneToErrorResultQuery

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCasesProneToErrorResultQuery
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


