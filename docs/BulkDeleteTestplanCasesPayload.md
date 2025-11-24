
# BulkDeleteTestplanCasesPayload


## Properties

Name | Type
------------ | -------------
`testcases` | Array&lt;number&gt;
`project` | number
`testplan` | number
`regression` | number

## Example

```typescript
import type { BulkDeleteTestplanCasesPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "testcases": null,
  "project": 1,
  "testplan": 1,
  "regression": 1,
} satisfies BulkDeleteTestplanCasesPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BulkDeleteTestplanCasesPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


