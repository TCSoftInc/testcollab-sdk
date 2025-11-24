
# LinkDefectPayload


## Properties

Name | Type
------------ | -------------
`defectKey` | string
`project` | number
`executedtestcase` | number
`stepNumber` | number
`defectId` | number

## Example

```typescript
import type { LinkDefectPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "defectKey": null,
  "project": 1,
  "executedtestcase": 1,
  "stepNumber": null,
  "defectId": 1,
} satisfies LinkDefectPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as LinkDefectPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


