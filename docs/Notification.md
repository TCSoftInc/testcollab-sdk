
# Notification


## Properties

Name | Type
------------ | -------------
`id` | number
`user` | number
`createdBy` | number
`label` | string
`project` | number
`company` | number
`systemName` | string
`additionalDetails` | string
`isRead` | boolean
`entityId` | number
`notificationgroup` | [NotificationGroups](NotificationGroups.md)
`createdAt` | string

## Example

```typescript
import type { Notification } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "user": 1,
  "createdBy": 1,
  "label": New test plan has been assigned to you,
  "project": 1,
  "company": 1,
  "systemName": APP,
  "additionalDetails": {},
  "isRead": true,
  "entityId": 1,
  "notificationgroup": null,
  "createdAt": 2019-04-30T17:11:24.000Z,
} satisfies Notification

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Notification
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


