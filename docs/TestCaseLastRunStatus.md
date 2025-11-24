
# TestCaseLastRunStatus

Last run status for test cases

## Properties

Name | Type
------------ | -------------
`skipped` | number
`failed` | number
`passed` | number
`unexecuted` | number

## Example

```typescript
import type { TestCaseLastRunStatus } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "skipped": 5,
  "failed": 20,
  "passed": 129,
  "unexecuted": 38,
} satisfies TestCaseLastRunStatus

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCaseLastRunStatus
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


