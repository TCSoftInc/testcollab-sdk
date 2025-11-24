
# ResultSummary

A summary of execution results. It includes counts for standard system statuses (unexecuted, passed, failed, skipped, blocked) which are always present. It can also include counts for any number of user-defined statuses. All statuses are represented as key-value pairs where the key is the status name (string) and the value is the count (number). 

## Properties

Name | Type
------------ | -------------
`unexecuted` | number
`passed` | number
`failed` | number
`skipped` | number
`blocked` | number

## Example

```typescript
import type { ResultSummary } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "unexecuted": 1,
  "passed": 10,
  "failed": 2,
  "skipped": 1,
  "blocked": 1,
} satisfies ResultSummary

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ResultSummary
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


