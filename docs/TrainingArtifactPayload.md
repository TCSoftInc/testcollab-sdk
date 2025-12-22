
# TrainingArtifactPayload


## Properties

Name | Type
------------ | -------------
`trainingSession` | number
`status` | string
`errorInfo` | string
`stepIndex` | number
`stepType` | string
`subStep` | number
`subStepTxt` | string
`imgFull` | string
`imgThumb` | string
`timestamp` | string
`browserLocation` | string
`otherInfoJson` | { [key: string]: any; }
`created` | string

## Example

```typescript
import type { TrainingArtifactPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "trainingSession": null,
  "status": null,
  "errorInfo": null,
  "stepIndex": null,
  "stepType": null,
  "subStep": null,
  "subStepTxt": null,
  "imgFull": null,
  "imgThumb": null,
  "timestamp": null,
  "browserLocation": null,
  "otherInfoJson": null,
  "created": null,
} satisfies TrainingArtifactPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TrainingArtifactPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


