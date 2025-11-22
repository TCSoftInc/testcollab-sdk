
# TestDatasetPayload


## Properties

Name | Type
------------ | -------------
`name` | string
`description` | string
`parameters` | [Array&lt;TestDatasetParameter&gt;](TestDatasetParameter.md)
`datarows` | string
`archived` | number
`project` | number

## Example

```typescript
import type { TestDatasetPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "name": Test dataset 1,
  "description": null,
  "parameters": null,
  "datarows": null,
  "archived": null,
  "project": null,
} satisfies TestDatasetPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestDatasetPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


