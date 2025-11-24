
# BulkActionResultDetail


## Properties

Name | Type
------------ | -------------
`status` | boolean
`id` | number
`message` | string

## Example

```typescript
import type { BulkActionResultDetail } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "status": true,
  "id": 1,
  "message": Action completed,
} satisfies BulkActionResultDetail

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BulkActionResultDetail
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


