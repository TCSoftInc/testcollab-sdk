
# TestCaseRequirementLinkResponse


## Properties

Name | Type
------------ | -------------
`status` | boolean
`testcase` | number
`requirement` | number

## Example

```typescript
import type { TestCaseRequirementLinkResponse } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "status": true,
  "testcase": 1826,
  "requirement": 79,
} satisfies TestCaseRequirementLinkResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCaseRequirementLinkResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


