
# TestCaseCopyPayload


## Properties

Name | Type
------------ | -------------
`testCase` | number
`project` | number

## Example

```typescript
import type { TestCaseCopyPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "testCase": 1,
  "project": 1,
} satisfies TestCaseCopyPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCaseCopyPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


