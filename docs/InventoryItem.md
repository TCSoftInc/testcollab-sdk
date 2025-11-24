
# InventoryItem


## Properties

Name | Type
------------ | -------------
`id` | string
`name` | string
`releaseDate` | Date
`manufacturer` | [Manufacturer](Manufacturer.md)

## Example

```typescript
import type { InventoryItem } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": d290f1ee-6c54-4b01-90e6-d701748f0851,
  "name": Widget Adapter,
  "releaseDate": 2016-08-29T09:12:33.001Z,
  "manufacturer": null,
} satisfies InventoryItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as InventoryItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


