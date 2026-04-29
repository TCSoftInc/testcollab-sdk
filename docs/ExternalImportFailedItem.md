
# ExternalImportFailedItem

A single source entity that failed to import

## Properties

Name | Type
------------ | -------------
`externalKey` | string
`entityType` | string
`reason` | string

## Example

```typescript
import type { ExternalImportFailedItem } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "externalKey": ABC-123,
  "entityType": testcase,
  "reason": TC API rejected payload: title is required,
} satisfies ExternalImportFailedItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExternalImportFailedItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


