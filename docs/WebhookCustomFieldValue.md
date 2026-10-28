
# WebhookCustomFieldValue


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`type` | string
`value` | any
`valueLabel` | string

## Example

```typescript
import type { WebhookCustomFieldValue } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "name": null,
  "type": null,
  "value": null,
  "valueLabel": null,
} satisfies WebhookCustomFieldValue

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookCustomFieldValue
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


