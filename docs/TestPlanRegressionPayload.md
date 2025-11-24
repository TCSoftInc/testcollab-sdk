
# TestPlanRegressionPayload


## Properties

Name | Type
------------ | -------------
`testCaseSelection` | Array&lt;string&gt;
`assignees` | Array&lt;number&gt;
`project` | number
`testplan` | number
`configurations` | Array&lt;number&gt;
`testcaseIds` | Array&lt;number&gt;

## Example

```typescript
import type { TestPlanRegressionPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "testCaseSelection": null,
  "assignees": null,
  "project": 1,
  "testplan": 1,
  "configurations": null,
  "testcaseIds": null,
} satisfies TestPlanRegressionPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanRegressionPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


