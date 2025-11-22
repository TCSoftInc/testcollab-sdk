
# CustomFieldCollectionOutput


## Properties

Name | Type
------------ | -------------
`type` | [CustomFieldType](CustomFieldType.md)
`id` | number
`name` | string
`label` | string
`valueLabel` | string
`color` | string
`value` | string

## Example

```typescript
import type { CustomFieldCollectionOutput } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "type": null,
  "id": 1,
  "name": custom_field_1,
  "label": Custom Field 1,
  "valueLabel": Custom field,
  "color": red,
  "value": Val 1,
} satisfies CustomFieldCollectionOutput

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CustomFieldCollectionOutput
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


