
# TestPlanFolderOrderProperty


## Properties

Name | Type
------------ | -------------
`dropToGap` | boolean
`dropPosition` | number
`draggedOnFolderId` | number
`targetFolderId` | Array&lt;number&gt;

## Example

```typescript
import type { TestPlanFolderOrderProperty } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "dropToGap": true,
  "dropPosition": 1,
  "draggedOnFolderId": 2,
  "targetFolderId": null,
} satisfies TestPlanFolderOrderProperty

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanFolderOrderProperty
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


