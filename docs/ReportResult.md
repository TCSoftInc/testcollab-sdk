
# ReportResult


## Properties

Name | Type
------------ | -------------
`status` | boolean
`data` | Array&lt;string&gt;
`message` | string
`queue` | [Queue](Queue.md)

## Example

```typescript
import type { ReportResult } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "status": true,
  "data": null,
  "message": Generating report,
  "queue": null,
} satisfies ReportResult

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReportResult
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


