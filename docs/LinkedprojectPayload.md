
# LinkedprojectPayload


## Properties

Name | Type
------------ | -------------
`imProjectKey` | string
`project` | number
`company` | number
`settings` | [LinkedProjectSettings](LinkedProjectSettings.md)
`imProjectId` | number
`createdBy` | number
`createdAt` | string
`imInstanceId` | string

## Example

```typescript
import type { LinkedprojectPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "imProjectKey": TestCase,
  "project": 1,
  "company": 1,
  "settings": null,
  "imProjectId": 1,
  "createdBy": 1,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "imInstanceId": null,
} satisfies LinkedprojectPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as LinkedprojectPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


