
# ProjectMini


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`archived` | boolean
`activity` | string
`totalTimeSpentLabel` | string
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { ProjectMini } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "name": Crowd Vox,
  "archived": false,
  "activity": 2017-06-05,
  "totalTimeSpentLabel": 54 min 12 sec,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "updatedAt": 2019-04-30T17:11:24.000Z,
} satisfies ProjectMini

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProjectMini
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


