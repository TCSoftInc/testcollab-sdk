
# CompanyPlanFeaturesInner

Plan features

## Properties

Name | Type
------------ | -------------
`name` | string
`displayName` | string
`allowed` | boolean
`limit` | number
`limitType` | string

## Example

```typescript
import type { CompanyPlanFeaturesInner } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "name": null,
  "displayName": null,
  "allowed": null,
  "limit": null,
  "limitType": null,
} satisfies CompanyPlanFeaturesInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CompanyPlanFeaturesInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


