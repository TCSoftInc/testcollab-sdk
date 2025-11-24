
# BulkCopyPayload


## Properties

Name | Type
------------ | -------------
`ids` | Array&lt;number&gt;
`project` | number

## Example

```typescript
import type { BulkCopyPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "ids": [1,2],
  "project": 3,
} satisfies BulkCopyPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BulkCopyPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


