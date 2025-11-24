
# MilestonePayload


## Properties

Name | Type
------------ | -------------
`name` | string
`dueDate` | number

## Example

```typescript
import type { MilestonePayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": V2 release,
  "dueDate": 1577836800,
} satisfies MilestonePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MilestonePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


