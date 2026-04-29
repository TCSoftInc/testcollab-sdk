
# ExternalImportProgress

Progress counters for the current import stage

## Properties

Name | Type
------------ | -------------
`current` | number
`total` | number
`percent` | number

## Example

```typescript
import type { ExternalImportProgress } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "current": 412,
  "total": 1247,
  "percent": 33,
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


