
# TestPlanFolderPayload


## Properties

Name | Type
------------ | -------------
`id` | number
`project` | number
`parentId` | number
`title` | string
`description` | string

## Example

```typescript
import type { TestPlanFolderPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "project": 1,
  "parentId": 1,
  "title": Sample,
  "description": My folder description,
} satisfies TestPlanFolderPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanFolderPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


