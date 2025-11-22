
# CustomFieldEditPayload


## Properties

Name | Type
------------ | -------------
`id` | number
`label` | string
`description` | string
`defaultValue` | string
`addToAllProjects` | boolean
`projects` | Array&lt;number&gt;
`search` | boolean
`isRequired` | boolean

## Example

```typescript
import type { CustomFieldEditPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "label": Custom Field,
  "description": This field does ABC etc.,
  "defaultValue": ABC,
  "addToAllProjects": false,
  "projects": [1,2,4],
  "search": true,
  "isRequired": true,
} satisfies CustomFieldEditPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CustomFieldEditPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


