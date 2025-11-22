
# ReusableStepPayload


## Properties

Name | Type
------------ | -------------
`project` | number
`name` | string
`steps` | [Array&lt;Step&gt;](Step.md)

## Example

```typescript
import type { ReusableStepPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "project": 1,
  "name": Login as a user,
  "steps": null,
} satisfies ReusableStepPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReusableStepPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


