
# ExternalImportRateLimitOptions

Optional per-service rate limit overrides for the import job

## Properties

Name | Type
------------ | -------------
`xrayGraphqlPerMin` | number
`jiraRestPerMin` | number

## Example

```typescript
import type { ExternalImportRateLimitOptions } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "xrayGraphqlPerMin": 50,
  "jiraRestPerMin": 30,
} satisfies ExternalImportRateLimitOptions

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExternalImportRateLimitOptions
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


