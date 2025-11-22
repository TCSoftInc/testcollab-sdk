
# DefectPayload


## Properties

Name | Type
------------ | -------------
`id` | number
`project` | number
`title` | string
`description` | string
`executedtestcase` | number
`stepNumber` | number
`_configuration` | string
`issueManager` | string

## Example

```typescript
import type { DefectPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "project": 1,
  "title": Test Failed - Test Case 1 - Step 1,
  "description": null,
  "executedtestcase": 1,
  "stepNumber": null,
  "_configuration": null,
  "issueManager": null,
} satisfies DefectPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DefectPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


