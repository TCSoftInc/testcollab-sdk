
# TestCasePassedBySuite

Object with suite name, number of test cases passed and color code value for heatmap

## Properties

Name | Type
------------ | -------------
`name` | string
`value` | number
`colorValue` | number

## Example

```typescript
import type { TestCasePassedBySuite } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "name": Basic Authorization,
  "value": 12,
  "colorValue": 75,
} satisfies TestCasePassedBySuite

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestCasePassedBySuite
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


