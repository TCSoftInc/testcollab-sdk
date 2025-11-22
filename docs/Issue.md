
# Issue


## Properties

Name | Type
------------ | -------------
`id` | number
`title` | string
`description` | string
`priority` | number
`status` | number
`attachments` | [Array&lt;Upload&gt;](Upload.md)
`customFields` | [Array&lt;CustomFieldCollectionOutput&gt;](CustomFieldCollectionOutput.md)
`createdAt` | string
`updatedAt` | string
`createdBy` | [UserMinified](UserMinified.md)
`updatedBy` | [UserMinified](UserMinified.md)

## Example

```typescript
import type { Issue } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "title": Issue 1,
  "description": null,
  "priority": null,
  "status": null,
  "attachments": null,
  "customFields": null,
  "createdAt": 2019-07-21T14:50:55.000Z,
  "updatedAt": 2019-08-21T14:50:55.000Z,
  "createdBy": null,
  "updatedBy": null,
} satisfies Issue

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Issue
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


