
# TrainingSession


## Properties

Name | Type
------------ | -------------
`id` | number
`testcase` | number
`testcaserevision` | number
`trainingUrl` | string
`customHeaders` | [Array&lt;QACCustomHeader&gt;](QACCustomHeader.md)
`triggeredBy` | number
`timeTaken` | number
`tokensConsumed` | number
`result` | string
`status` | string
`videoUrl` | string
`project` | number
`company` | number
`queue` | number
`createdAt` | Date

## Example

```typescript
import type { TrainingSession } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 3201,
  "testcase": 182,
  "testcaserevision": 9,
  "trainingUrl": https://example.com,
  "customHeaders": null,
  "triggeredBy": 53,
  "timeTaken": 38.5,
  "tokensConsumed": 1245,
  "result": passed,
  "status": inprogress,
  "videoUrl": https://example.com/training_session_3201.mp4,
  "project": 11,
  "company": 3,
  "queue": 845,
  "createdAt": 2025-11-04T09:23:11Z,
} satisfies TrainingSession

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TrainingSession
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


