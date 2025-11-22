
# NotificationsInner


## Properties

Name | Type
------------ | -------------
`systemName` | string
`label` | string
`user` | number
`createdBy` | number

## Example

```typescript
import type { NotificationsInner } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "systemName": testCaseFailed,
  "label": When test case fails,
  "user": 1,
  "createdBy": 1,
} satisfies NotificationsInner

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as NotificationsInner
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


