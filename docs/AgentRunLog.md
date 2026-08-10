
# AgentRunLog


## Properties

Name | Type
------------ | -------------
`id` | number
`agentRun` | number
`seq` | number
`level` | string
`message` | string
`createdAt` | string

## Example

```typescript
import type { AgentRunLog } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "agentRun": 1,
  "seq": 12,
  "level": info,
  "message": Fetched test plan 12 with 8 cases,
  "createdAt": 2026-08-05T17:11:24.000Z,
} satisfies AgentRunLog

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AgentRunLog
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


