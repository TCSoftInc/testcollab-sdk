
# NotificationGroups


## Properties

Name | Type
------------ | -------------
`group` | string
`notifications` | [Array&lt;NotificationsInner&gt;](NotificationsInner.md)

## Example

```typescript
import type { NotificationGroups } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "group": TestCase,
  "notifications": null,
} satisfies NotificationGroups

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as NotificationGroups
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


