
# ExternalImportSourceProjectCounts

Per-entity counts in a source project (used by the project picker UI). Fields may be omitted when the source adapter cannot provide an exact count cheaply.

## Properties

Name | Type
------------ | -------------
`testCases` | number
`testSets` | number
`testPlans` | number
`folders` | number

## Example

```typescript
import type { ExternalImportSourceProjectCounts } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "testCases": 1247,
  "testSets": 34,
  "testPlans": 12,
  "folders": 89,
} satisfies ExternalImportSourceProjectCounts

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExternalImportSourceProjectCounts
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


