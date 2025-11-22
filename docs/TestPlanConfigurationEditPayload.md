
# TestPlanConfigurationEditPayload


## Properties

Name | Type
------------ | -------------
`parameters` | [Array&lt;ConfigCombination&gt;](ConfigCombination.md)
`id` | number
`assignedTo` | number

## Example

```typescript
import type { TestPlanConfigurationEditPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "parameters": null,
  "id": 1,
  "assignedTo": 1,
} satisfies TestPlanConfigurationEditPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanConfigurationEditPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


