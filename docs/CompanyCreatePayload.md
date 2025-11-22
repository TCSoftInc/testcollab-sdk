
# CompanyCreatePayload


## Properties

Name | Type
------------ | -------------
`name` | string
`size` | number
`phone` | string
`country` | string
`countryCode` | string

## Example

```typescript
import type { CompanyCreatePayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "name": Test Collab Software Inc.,
  "size": 10,
  "phone": +1 613 555 0107,
  "country": Canada,
  "countryCode": CA,
} satisfies CompanyCreatePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CompanyCreatePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


