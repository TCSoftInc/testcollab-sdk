
# TestCaseQacTimeoutPayload


## Properties

Name | Type
------------ | -------------
`testcase` | number
`project` | number
`qacTimeout` | number

## Example

```typescript
import type { TestCaseQacTimeoutPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "testcase": 1,
  "project": 1,
  "qacTimeout": 1,
} satisfies TestCaseQacTimeoutPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCaseQacTimeoutPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


