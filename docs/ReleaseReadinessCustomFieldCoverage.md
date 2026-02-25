
# ReleaseReadinessCustomFieldCoverage

Coverage breakdown for a single custom field. Groups test cases by their custom field value and shows execution statistics per group. Supports both test case and test plan custom fields. 

## Properties

Name | Type
------------ | -------------
`fieldId` | number
`fieldLabel` | string
`fieldType` | string
`entity` | string
`groups` | [Array&lt;ReleaseReadinessCustomFieldGroup&gt;](ReleaseReadinessCustomFieldGroup.md)

## Example

```typescript
import type { ReleaseReadinessCustomFieldCoverage } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "fieldId": 5,
  "fieldLabel": Priority Level,
  "fieldType": dropdown,
  "entity": TestCase,
  "groups": null,
} satisfies ReleaseReadinessCustomFieldCoverage

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReleaseReadinessCustomFieldCoverage
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


