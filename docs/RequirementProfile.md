
# RequirementProfile


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`requirementManager` | string
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { RequirementProfile } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "name": Main bug tracker,
  "requirementManager": jira,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "updatedAt": 2019-04-30T17:11:24.000Z,
} satisfies RequirementProfile

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RequirementProfile
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


