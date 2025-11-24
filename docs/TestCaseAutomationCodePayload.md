
# TestCaseAutomationCodePayload


## Properties

Name | Type
------------ | -------------
`testcase` | number
`testcaserevision` | number
`project` | number
`code` | string
`mode` | string
`automationStatus` | number
`automationInfo` | string

## Example

```typescript
import type { TestCaseAutomationCodePayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "testcase": 1,
  "testcaserevision": 1,
  "project": 1,
  "code": null,
  "mode": null,
  "automationStatus": 1,
  "automationInfo": null,
} satisfies TestCaseAutomationCodePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCaseAutomationCodePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


