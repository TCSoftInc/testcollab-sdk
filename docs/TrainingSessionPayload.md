
# TrainingSessionPayload


## Properties

Name | Type
------------ | -------------
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
`created` | Date
`project` | number
`company` | number
`queue` | number

## Example

```typescript
import type { TrainingSessionPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "testcase": null,
  "testcaserevision": null,
  "trainingUrl": null,
  "customHeaders": null,
  "triggeredBy": null,
  "timeTaken": null,
  "tokensConsumed": null,
  "result": null,
  "status": null,
  "videoUrl": null,
  "created": null,
  "project": null,
  "company": null,
  "queue": null,
} satisfies TrainingSessionPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TrainingSessionPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


