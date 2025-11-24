
# CustomField


## Properties

Name | Type
------------ | -------------
`id` | number
`sortOrder` | number
`name` | string
`label` | string
`entity` | string
`type` | [CustomFieldType](CustomFieldType.md)
`defaultValue` | string
`isRequired` | boolean
`addToAllProjects` | boolean
`projects` | Array&lt;number&gt;
`search` | boolean
`extra` | [CustomFieldExtraProps](CustomFieldExtraProps.md)
`company` | number
`description` | string
`isSortable` | boolean

## Example

```typescript
import type { CustomField } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "sortOrder": 1,
  "name": custom_field_1,
  "label": Custom Field 1,
  "entity": TestCase,
  "type": null,
  "defaultValue": My value,
  "isRequired": true,
  "addToAllProjects": false,
  "projects": [1,2,4],
  "search": true,
  "extra": null,
  "company": 1,
  "description": Custom field description,
  "isSortable": true,
} satisfies CustomField

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CustomField
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


