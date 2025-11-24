
# AddSuitePayload


## Properties

Name | Type
------------ | -------------
`parentId` | number
`title` | string
`description` | string
`project` | number

## Example

```typescript
import type { AddSuitePayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "parentId": 2,
  "title": Suite 1,
  "description": My suite,
  "project": 1,
} satisfies AddSuitePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AddSuitePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


