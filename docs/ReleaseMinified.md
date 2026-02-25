
# ReleaseMinified


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`status` | string
`targetDate` | string
`createdAt` | string

## Example

```typescript
import type { ReleaseMinified } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "name": v2.4.0,
  "status": in_progress,
  "targetDate": 2025-03-15,
  "createdAt": 2025-02-11T10:00:00.000Z,
} satisfies ReleaseMinified

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReleaseMinified
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


