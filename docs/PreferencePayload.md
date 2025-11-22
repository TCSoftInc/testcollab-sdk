
# PreferencePayload


## Properties

Name | Type
------------ | -------------
`notification` | string
`selectionType` | string
`hide` | string

## Example

```typescript
import type { PreferencePayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "notification": Deleting test cases,
  "selectionType": null,
  "hide": yes/no/24hours,
} satisfies PreferencePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PreferencePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


