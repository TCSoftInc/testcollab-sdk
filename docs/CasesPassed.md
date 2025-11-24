
# CasesPassed

The number of test cases passed v/s number of cases assigned

## Properties

Name | Type
------------ | -------------
`total` | number
`passed` | number

## Example

```typescript
import type { CasesPassed } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "total": 5,
  "passed": 3,
} satisfies CasesPassed

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CasesPassed
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


