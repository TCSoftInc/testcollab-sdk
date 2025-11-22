
# GenericFolderTree


## Properties

Name | Type
------------ | -------------
`id` | number
`title` | string
`folderitemcount` | number
`parentId` | number
`description` | string
`createdBy` | number
`children` | [Array&lt;GenericFolderTree&gt;](GenericFolderTree.md)

## Example

```typescript
import type { GenericFolderTree } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 2,
  "title": Folder 1,
  "folderitemcount": 2,
  "parentId": 0,
  "description": Folder description,
  "createdBy": null,
  "children": null,
} satisfies GenericFolderTree

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GenericFolderTree
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


