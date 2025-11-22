
# CustomerAccountInfomation


## Properties

Name | Type
------------ | -------------
`id` | string
`firstName` | string
`lastName` | string
`company` | string
`email` | string
`phone` | string
`addressLine1` | string
`addressLine2` | string
`city` | string
`region` | string
`postalCode` | string
`language` | string
`country` | string
`url` | string

## Example

```typescript
import type { CustomerAccountInfomation } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": klnNfOqcRRmjERH_1gBVUQ,
  "firstName": John,
  "lastName": Carter,
  "company": ABC Company,
  "email": null,
  "phone": null,
  "addressLine1": null,
  "addressLine2": null,
  "city": null,
  "region": null,
  "postalCode": null,
  "language": en,
  "country": IN,
  "url": https://testcollab.test.onfastspring.com/account,
} satisfies CustomerAccountInfomation

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CustomerAccountInfomation
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


