
# ProjectUserRemoveResult


## Properties

Name | Type
------------ | -------------
`status` | boolean
`queue` | number
`impact` | [ProjectUserRemovalImpact](ProjectUserRemovalImpact.md)

## Example

```typescript
import type { ProjectUserRemoveResult } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "status": true,
  "queue": 981,
  "impact": null,
} satisfies ProjectUserRemoveResult

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ProjectUserRemoveResult
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


