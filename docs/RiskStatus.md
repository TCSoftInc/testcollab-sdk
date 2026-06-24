
# RiskStatus


## Properties

Name | Type
------------ | -------------
`id` | number
`project` | number
`name` | string
`color` | string
`isSystem` | boolean
`isClosed` | boolean
`position` | number
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { RiskStatus } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "project": 1,
  "name": Mitigating,
  "color": #2d6bcf,
  "isSystem": false,
  "isClosed": false,
  "position": 3,
  "createdAt": 2026-04-30T17:11:24.000Z,
  "updatedAt": 2026-04-30T17:11:24.000Z,
} satisfies RiskStatus

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RiskStatus
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


