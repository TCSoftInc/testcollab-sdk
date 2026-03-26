
# ProjectSecret


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`description` | string
`project` | number
`createdBy` | number
`updatedBy` | number
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { ProjectSecret } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "name": LOGIN_PASSWORD,
  "description": Login password for staging environment,
  "project": 1,
  "createdBy": 1,
  "updatedBy": 1,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "updatedAt": 2019-04-30T17:11:24.000Z,
} satisfies ProjectSecret

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProjectSecret
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


