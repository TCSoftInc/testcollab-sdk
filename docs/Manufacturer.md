
# Manufacturer


## Properties

Name | Type
------------ | -------------
`name` | string
`homePage` | string
`phone` | string

## Example

```typescript
import type { Manufacturer } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": ACME Corporation,
  "homePage": https://www.acme-corp.com,
  "phone": 408-867-5309,
} satisfies Manufacturer

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Manufacturer
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


