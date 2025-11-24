
# ExecutedTestCaseValidatePayload


## Properties

Name | Type
------------ | -------------
`project` | number
`testplan` | number
`execcaseIds` | Array&lt;number&gt;
`configId` | number
`status` | boolean
`comment` | string

## Example

```typescript
import type { ExecutedTestCaseValidatePayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "project": null,
  "testplan": null,
  "execcaseIds": null,
  "configId": null,
  "status": null,
  "comment": null,
} satisfies ExecutedTestCaseValidatePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExecutedTestCaseValidatePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


