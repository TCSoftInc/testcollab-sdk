
# ExternalImportCreateResult


## Properties

Name | Type
------------ | -------------
`importId` | number
`queueId` | number
`status` | string

## Example

```typescript
import type { ExternalImportCreateResult } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "importId": 18,
  "queueId": 9821,
  "status": pending,
} satisfies ExternalImportCreateResult

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExternalImportCreateResult
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


