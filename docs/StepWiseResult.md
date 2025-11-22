
# StepWiseResult


## Properties

Name | Type
------------ | -------------
`stepIndex` | number
`step` | string
`expectedResult` | string
`status` | string
`comment` | string
`mentions` | Array&lt;string&gt;
`attachments` | Array&lt;string&gt;

## Example

```typescript
import type { StepWiseResult } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "stepIndex": 1,
  "step": Step 1,
  "expectedResult": Expected result 1,
  "status": unexecuted,
  "comment": My comment,
  "mentions": null,
  "attachments": null,
} satisfies StepWiseResult

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as StepWiseResult
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


