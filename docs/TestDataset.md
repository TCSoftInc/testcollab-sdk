
# TestDataset


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`description` | string
`parameters` | [Array&lt;TestDatasetParameter&gt;](TestDatasetParameter.md)
`datarows` | string
`createdAt` | string
`updatedAt` | string
`createdBy` | [UserMinified](UserMinified.md)
`archived` | number

## Example

```typescript
import type { TestDataset } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "name": Test dataset 1,
  "description": null,
  "parameters": null,
  "datarows": null,
  "createdAt": 2019-07-21T14:50:55.000Z,
  "updatedAt": 2019-08-21T14:50:55.000Z,
  "createdBy": null,
  "archived": null,
} satisfies TestDataset

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestDataset
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


