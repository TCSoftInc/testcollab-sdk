
# BuildMinified


## Properties

Name | Type
------------ | -------------
`id` | number
`version` | string
`environment` | string
`source` | string
`releaseDate` | string
`createdAt` | string

## Example

```typescript
import type { BuildMinified } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "version": v2.14.1,
  "environment": Production,
  "source": manual,
  "releaseDate": 2026-06-27,
  "createdAt": 2026-06-27T15:04:00.000Z,
} satisfies BuildMinified

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BuildMinified
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


