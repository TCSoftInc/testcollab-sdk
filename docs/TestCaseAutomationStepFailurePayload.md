
# TestCaseAutomationStepFailurePayload


## Properties

Name | Type
------------ | -------------
`testcase` | number
`testcaserevision` | number
`project` | number
`step` | string
`stepCounter` | number
`tcStepCounter` | number
`errorDescription` | string

## Example

```typescript
import type { TestCaseAutomationStepFailurePayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "testcase": 1,
  "testcaserevision": 1,
  "project": 1,
  "step": null,
  "stepCounter": null,
  "tcStepCounter": null,
  "errorDescription": null,
} satisfies TestCaseAutomationStepFailurePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCaseAutomationStepFailurePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


