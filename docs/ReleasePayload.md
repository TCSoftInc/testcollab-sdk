
# ReleasePayload


## Properties

Name | Type
------------ | -------------
`name` | string
`description` | string
`status` | string
`targetDate` | string
`releaseDate` | string
`goNoGoThreshold` | [ReleaseGoNoGoThreshold](.md)
`isPublic` | boolean
`project` | number
`testPlans` | Array&lt;number&gt;
`requirements` | Array&lt;number&gt;

## Example

```typescript
import type { ReleasePayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": v2.4.0,
  "description": Sprint 23 release with payment module updates,
  "status": planned,
  "targetDate": 2025-03-15,
  "releaseDate": 2025-03-14,
  "goNoGoThreshold": null,
  "isPublic": false,
  "project": 1,
  "testPlans": [1,5,12],
  "requirements": [10,20,35],
} satisfies ReleasePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReleasePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


