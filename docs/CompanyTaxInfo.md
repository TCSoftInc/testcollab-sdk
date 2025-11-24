
# CompanyTaxInfo


## Properties

Name | Type
------------ | -------------
`exempt` | boolean
`taxRate` | number

## Example

```typescript
import type { CompanyTaxInfo } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "exempt": false,
  "taxRate": 10,
} satisfies CompanyTaxInfo

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CompanyTaxInfo
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


