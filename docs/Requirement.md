
# Requirement


## Properties

Name | Type
------------ | -------------
`id` | number
`title` | string
`requirementManager` | string
`requirementId` | string
`requirementKey` | string
`requirementUrl` | string
`project` | number
`status` | number
`reqInfo` | string
`testcaseCount` | number
`customFields` | [Array&lt;CustomFieldCollectionOutput&gt;](CustomFieldCollectionOutput.md)
`requirementFolder` | [GenericFolder](GenericFolder.md)
`attachments` | [Array&lt;Upload&gt;](Upload.md)
`description` | string
`createdAt` | string
`updatedAt` | string
`createdBy` | [UserMinified](UserMinified.md)

## Example

```typescript
import type { Requirement } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 2,
  "title": null,
  "requirementManager": null,
  "requirementId": null,
  "requirementKey": null,
  "requirementUrl": null,
  "project": 1,
  "status": null,
  "reqInfo": null,
  "testcaseCount": null,
  "customFields": null,
  "requirementFolder": null,
  "attachments": null,
  "description": null,
  "createdAt": 2019-07-21T14:50:55.000Z,
  "updatedAt": 2019-08-21T14:50:55.000Z,
  "createdBy": null,
} satisfies Requirement

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Requirement
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


