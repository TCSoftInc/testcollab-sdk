
# BulkActionResult


## Properties

Name | Type
------------ | -------------
`status` | boolean
`affected` | number
`details` | [Array&lt;BulkActionResultDetail&gt;](BulkActionResultDetail.md)
`message` | string
`queue` | [Queue](Queue.md)

## Example

```typescript
import type { BulkActionResult } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "status": true,
  "affected": 1,
  "details": null,
  "message": Action completed,
  "queue": null,
} satisfies BulkActionResult

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BulkActionResult
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


