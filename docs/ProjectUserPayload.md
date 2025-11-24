
# ProjectUserPayload


## Properties

Name | Type
------------ | -------------
`id` | number
`project` | number
`user` | number
`role` | number

## Example

```typescript
import type { ProjectUserPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "project": 1,
  "user": 1,
  "role": 1,
} satisfies ProjectUserPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProjectUserPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


