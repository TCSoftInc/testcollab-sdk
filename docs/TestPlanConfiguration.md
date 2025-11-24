
# TestPlanConfiguration


## Properties

Name | Type
------------ | -------------
`id` | number
`parameters` | [Array&lt;ConfigCombination&gt;](ConfigCombination.md)
`assignedTo` | [UserMinified](UserMinified.md)

## Example

```typescript
import type { TestPlanConfiguration } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "parameters": null,
  "assignedTo": null,
} satisfies TestPlanConfiguration

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanConfiguration
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


