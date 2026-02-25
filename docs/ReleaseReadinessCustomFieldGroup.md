
# ReleaseReadinessCustomFieldGroup

Coverage data for a single value/group within a custom field. 

## Properties

Name | Type
------------ | -------------
`value` | string
`label` | string
`color` | string
`total` | number
`executed` | number
`passed` | number
`failed` | number
`passRate` | number

## Example

```typescript
import type { ReleaseReadinessCustomFieldGroup } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "value": high_priority,
  "label": High Priority,
  "color": #f5222d,
  "total": 15,
  "executed": 12,
  "passed": 10,
  "failed": 2,
  "passRate": 83.3,
} satisfies ReleaseReadinessCustomFieldGroup

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReleaseReadinessCustomFieldGroup
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


