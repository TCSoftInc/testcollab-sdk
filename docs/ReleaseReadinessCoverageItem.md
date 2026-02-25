
# ReleaseReadinessCoverageItem

Test coverage for a single suite/module within the release. Supports tree structure — parent suites aggregate totals from children. 

## Properties

Name | Type
------------ | -------------
`suiteId` | number
`suiteTitle` | string
`total` | number
`executed` | number
`passed` | number
`failed` | number
`passRate` | number
`children` | [Array&lt;ReleaseReadinessCoverageItem&gt;](ReleaseReadinessCoverageItem.md)

## Example

```typescript
import type { ReleaseReadinessCoverageItem } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "suiteId": 42,
  "suiteTitle": Payment Module,
  "total": 25,
  "executed": 20,
  "passed": 18,
  "failed": 2,
  "passRate": 90,
  "children": null,
} satisfies ReleaseReadinessCoverageItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReleaseReadinessCoverageItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


