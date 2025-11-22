
# FolderTree


## Properties

Name | Type
------------ | -------------
`id` | number
`title` | string
`testplancount` | number
`parentId` | number
`description` | string
`createdBy` | number
`children` | [Array&lt;FolderTree&gt;](FolderTree.md)

## Example

```typescript
import type { FolderTree } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 2,
  "title": Folder 1,
  "testplancount": 2,
  "parentId": 0,
  "description": Folder description,
  "createdBy": null,
  "children": null,
} satisfies FolderTree

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as FolderTree
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


