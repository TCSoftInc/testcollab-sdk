
# TestCaseAutomationProgressPayload


## Properties

Name | Type
------------ | -------------
`testcase` | number
`testcaserevision` | number
`project` | number
`code` | string
`step` | string
`automationStatus` | number
`stepNumber` | number
`stepType` | string
`stepStatus` | string
`stepError` | string
`stepImages` | Array&lt;string&gt;
`trainingVideoUrl` | string

## Example

```typescript
import type { TestCaseAutomationProgressPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "testcase": 1,
  "testcaserevision": 1,
  "project": 1,
  "code": null,
  "step": null,
  "automationStatus": 1,
  "stepNumber": null,
  "stepType": null,
  "stepStatus": null,
  "stepError": null,
  "stepImages": null,
  "trainingVideoUrl": https://example.com/training_video.mp4,
} satisfies TestCaseAutomationProgressPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCaseAutomationProgressPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


