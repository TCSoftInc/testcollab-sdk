
# BuildRiskCoverageItem

A single risk\'s coverage in a build (TCV-6726).

## Properties

Name | Type
------------ | -------------
`id` | number
`displayNumber` | number
`title` | string
`exposureBand` | string
`casesRun` | number
`covered` | boolean

## Example

```typescript
import type { BuildRiskCoverageItem } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 4,
  "displayNumber": 4,
  "title": Duplicate payment on retry,
  "exposureBand": high,
  "casesRun": 6,
  "covered": true,
} satisfies BuildRiskCoverageItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BuildRiskCoverageItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


