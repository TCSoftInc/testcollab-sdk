
# ExternalImportProgress

Progress counters for the current import stage

## Properties

Name | Type
------------ | -------------
`current` | number
`total` | number
`percent` | number
`detail` | { [key: string]: any; }

## Example

```typescript
import type { ExternalImportProgress } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "current": 412,
  "total": 1247,
  "percent": 33,
  "detail": {"phase":"test_cases","current_plan_name":"Checkout regression","plans_current":12,"plans_total":2860,"test_cases_current":150,"test_cases_total":420},
} satisfies ExternalImportProgress

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExternalImportProgress
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


