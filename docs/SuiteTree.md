
# SuiteTree


## Properties

Name | Type
------------ | -------------
`id` | number
`title` | string
`suitecount` | number
`createdBy` | number
`testcasecount` | number
`alltestcasecount` | number
`children` | [Array&lt;SuiteTree&gt;](SuiteTree.md)
`isReference` | boolean
`sourceId` | number
`sourceProject` | number
`isMainLink` | boolean

## Example

```typescript
import type { SuiteTree } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "title": Suite 1,
  "suitecount": 23,
  "createdBy": 23,
  "testcasecount": 23,
  "alltestcasecount": 23,
  "children": null,
  "isReference": false,
  "sourceId": 1,
  "sourceProject": 1,
  "isMainLink": false,
} satisfies SuiteTree

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SuiteTree
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


