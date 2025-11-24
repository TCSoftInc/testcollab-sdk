
# MarkNotificationPayload


## Properties

Name | Type
------------ | -------------
`company` | number
`notification` | number

## Example

```typescript
import type { MarkNotificationPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "company": 1,
  "notification": 1,
} satisfies MarkNotificationPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MarkNotificationPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


