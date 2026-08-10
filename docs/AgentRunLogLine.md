
# AgentRunLogLine


## Properties

Name | Type
------------ | -------------
`seq` | number
`level` | string
`message` | string

## Example

```typescript
import type { AgentRunLogLine } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "seq": 12,
  "level": info,
  "message": Fetched test plan 12 with 8 cases,
} satisfies AgentRunLogLine

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AgentRunLogLine
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


