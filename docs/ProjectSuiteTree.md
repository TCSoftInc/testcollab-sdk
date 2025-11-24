
# ProjectSuiteTree


## Properties

Name | Type
------------ | -------------
`id` | number
`project` | [ProjectMini](ProjectMini.md)
`tree` | [Array&lt;SuiteTree&gt;](SuiteTree.md)

## Example

```typescript
import type { ProjectSuiteTree } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "project": null,
  "tree": null,
} satisfies ProjectSuiteTree

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProjectSuiteTree
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


