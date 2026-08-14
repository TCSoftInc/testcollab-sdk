
# RiskVerification

Rollup of the last result of every test case linked to the risk. Coverage says a risk has tests; verification says what those tests reported. Counts come from each linked test case\'s latest execution anywhere in the project. 

## Properties

Name | Type
------------ | -------------
`state` | string
`passed` | number
`failed` | number
`notVerified` | number

## Example

```typescript
import type { RiskVerification } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "state": failed,
  "passed": 3,
  "failed": 1,
  "notVerified": 2,
} satisfies RiskVerification

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RiskVerification
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


