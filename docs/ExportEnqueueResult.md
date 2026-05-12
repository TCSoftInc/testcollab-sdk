
# ExportEnqueueResult

Response when an export request is accepted. The export runs asynchronously on the background queue runner. Clients poll GET /queues/{id} until status is 2 (success) or 3 (failure); on success, queue.results contains { url, fileId, filename, size, rowCount }.

## Properties

Name | Type
------------ | -------------
`queueId` | number

## Example

```typescript
import type { ExportEnqueueResult } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "queueId": 12345,
} satisfies ExportEnqueueResult

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExportEnqueueResult
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


