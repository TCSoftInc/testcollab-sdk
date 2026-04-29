
# ExternalImportOptions

Per-import behavioural options

## Properties

Name | Type
------------ | -------------
`skipDuplicates` | boolean
`dedupThreshold` | number
`dedupSameRepositoryOnly` | boolean
`defaultTestPlanAssignee` | number
`rateLimits` | [ExternalImportRateLimitOptions](ExternalImportRateLimitOptions.md)

## Example

```typescript
import type { ExternalImportOptions } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "skipDuplicates": true,
  "dedupThreshold": 0.55,
  "dedupSameRepositoryOnly": true,
  "defaultTestPlanAssignee": null,
  "rateLimits": null,
} satisfies ExternalImportOptions

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExternalImportOptions
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


