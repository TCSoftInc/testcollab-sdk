
# Linkedproject


## Properties

Name | Type
------------ | -------------
`imProjectKey` | string
`project` | [Project](Project.md)
`company` | [Company](Company.md)
`settings` | [LinkedProjectSettings](LinkedProjectSettings.md)
`imProjectId` | number
`createdBy` | [User](User.md)
`createdAt` | string

## Example

```typescript
import type { Linkedproject } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "imProjectKey": TestCase,
  "project": null,
  "company": null,
  "settings": null,
  "imProjectId": 1,
  "createdBy": null,
  "createdAt": 2019-04-30T17:11:24.000Z,
} satisfies Linkedproject

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Linkedproject
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


