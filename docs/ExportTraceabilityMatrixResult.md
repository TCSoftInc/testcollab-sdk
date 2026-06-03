
# ExportTraceabilityMatrixResult

Result of a traceability matrix export enqueue request. The export runs asynchronously on the background queue runner. Clients poll GET /queues/{id} until status is 2 or 3; on success, queue.results contains the generated CSV URL. 

## Properties

Name | Type
------------ | -------------
`queueId` | number
`headerRow` | string
`rows` | Array&lt;string&gt;
`totalRows` | number
`queue` | [Queue](Queue.md)

## Example

```typescript
import type { ExportTraceabilityMatrixResult } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "queueId": null,
  "headerRow": null,
  "rows": null,
  "totalRows": null,
  "queue": null,
} satisfies ExportTraceabilityMatrixResult

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExportTraceabilityMatrixResult
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


