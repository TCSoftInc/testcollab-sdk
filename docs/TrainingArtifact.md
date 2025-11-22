
# TrainingArtifact


## Properties

Name | Type
------------ | -------------
`id` | number
`trainingSession` | number
`status` | string
`errorInfo` | string
`stepIndex` | number
`stepType` | string
`subStep` | number
`subStepTxt` | string
`imgFull` | string
`imgThumb` | string
`timestamp` | Date
`browserLocation` | string
`otherInfoJson` | { [key: string]: any; }
`createdAt` | Date

## Example

```typescript
import type { TrainingArtifact } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 91015,
  "trainingSession": 3201,
  "status": pass,
  "errorInfo": Selector .btn-submit not found,
  "stepIndex": 4,
  "stepType": i,
  "subStep": 2,
  "subStepTxt": Verify the welcome banner,
  "imgFull": https://cdn.example.com/training/3201/step_4_full.png,
  "imgThumb": https://cdn.example.com/training/3201/step_4_thumb.png,
  "timestamp": 2025-11-04T09:25:44Z,
  "browserLocation": https://example.com/cart,
  "otherInfoJson": null,
  "createdAt": 2025-11-04T09:26:01Z,
} satisfies TrainingArtifact

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TrainingArtifact
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


