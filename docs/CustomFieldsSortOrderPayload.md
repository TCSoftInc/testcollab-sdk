
# CustomFieldsSortOrderPayload


## Properties

Name | Type
------------ | -------------
`company` | number
`id` | number
`entity` | string
`oldPosition` | number
`newPosition` | number

## Example

```typescript
import type { CustomFieldsSortOrderPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "company": 1,
  "id": 1,
  "entity": TestCase,
  "oldPosition": 1,
  "newPosition": 2,
} satisfies CustomFieldsSortOrderPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CustomFieldsSortOrderPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


