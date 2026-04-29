
# ActivityFieldChange

A single field-level change within an activity

## Properties

Name | Type
------------ | -------------
`field` | string
`label` | string
`type` | string
`oldValue` | string
`newValue` | string

## Example

```typescript
import type { ActivityFieldChange } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "field": assigned_to,
  "label": Assigned To,
  "type": user,
  "oldValue": 42,
  "newValue": 55,
} satisfies ActivityFieldChange

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ActivityFieldChange
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


