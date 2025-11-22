
# TestPlanConfigurationPayload


## Properties

Name | Type
------------ | -------------
`parameters` | Array&lt;Array&lt;ConfigCombination&gt;&gt;
`project` | number
`testplan` | number

## Example

```typescript
import type { TestPlanConfigurationPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "parameters": null,
  "project": 1,
  "testplan": 1,
} satisfies TestPlanConfigurationPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanConfigurationPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


