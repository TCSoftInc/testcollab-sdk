
# AgentRunLogPayload


## Properties

Name | Type
------------ | -------------
`agentRun` | number
`lines` | [Array&lt;AgentRunLogLine&gt;](AgentRunLogLine.md)

## Example

```typescript
import type { AgentRunLogPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "agentRun": 1,
  "lines": null,
} satisfies AgentRunLogPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AgentRunLogPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


