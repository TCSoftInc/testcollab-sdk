
# NotificationPreferencePayload


## Properties

Name | Type
------------ | -------------
`preferences` | [Array&lt;PreferencePayload&gt;](PreferencePayload.md)
`user` | number
`company` | number

## Example

```typescript
import type { NotificationPreferencePayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "preferences": null,
  "user": 1,
  "company": 10,
} satisfies NotificationPreferencePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as NotificationPreferencePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


