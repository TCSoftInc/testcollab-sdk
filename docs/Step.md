
# Step


## Properties

Name | Type
------------ | -------------
`step` | string
`expectedResult` | string
`reusableStepId` | number

## Example

```typescript
import type { Step } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "step": Step 1,
  "expectedResult": Expected result 1,
  "reusableStepId": null,
} satisfies Step

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Step
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


