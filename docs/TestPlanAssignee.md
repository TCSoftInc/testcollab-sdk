
# TestPlanAssignee


## Properties

Name | Type
------------ | -------------
`id` | number
`username` | string
`name` | string
`results` | [Array&lt;ConfigWiseResult&gt;](ConfigWiseResult.md)

## Example

```typescript
import type { TestPlanAssignee } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "username": shritig,
  "name": Abhimanyu Grover,
  "results": null,
} satisfies TestPlanAssignee

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanAssignee
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


