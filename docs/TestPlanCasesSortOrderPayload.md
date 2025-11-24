
# TestPlanCasesSortOrderPayload


## Properties

Name | Type
------------ | -------------
`project` | number
`testplan` | number
`ids` | Array&lt;number&gt;
`oldPosition` | number
`newPosition` | number

## Example

```typescript
import type { TestPlanCasesSortOrderPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "project": 1,
  "testplan": null,
  "ids": [1,2,3],
  "oldPosition": 1,
  "newPosition": 2,
} satisfies TestPlanCasesSortOrderPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanCasesSortOrderPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


