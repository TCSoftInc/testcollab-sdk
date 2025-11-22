
# StripeTaxInfo


## Properties

Name | Type
------------ | -------------
`name` | string
`taxRate` | number

## Example

```typescript
import type { StripeTaxInfo } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "name": Sales Tax,
  "taxRate": 5,
} satisfies StripeTaxInfo

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as StripeTaxInfo
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


