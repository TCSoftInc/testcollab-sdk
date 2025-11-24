
# TaxRate


## Properties

Name | Type
------------ | -------------
`id` | string
`displayName` | string
`inclusive` | boolean
`percentage` | number

## Example

```typescript
import type { TaxRate } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": tax_kdfj4jf49r,
  "displayName": null,
  "inclusive": false,
  "percentage": 5,
} satisfies TaxRate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TaxRate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


