
# ExternalImportTestConnectionResult


## Properties

Name | Type
------------ | -------------
`ok` | boolean
`tokenTtlSeconds` | number
`projectCount` | number

## Example

```typescript
import type { ExternalImportTestConnectionResult } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "ok": true,
  "tokenTtlSeconds": 86400,
  "projectCount": 23,
} satisfies ExternalImportTestConnectionResult

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExternalImportTestConnectionResult
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


