
# AgentRunInputs


## Properties

Name | Type
------------ | -------------
`agentRun` | number
`prompt` | string
`customPrompt` | string
`manifest` | [AgentRunManifest](AgentRunManifest.md)

## Example

```typescript
import type { AgentRunInputs } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "agentRun": 1,
  "prompt": You are a TestCollab QA agent...
,
  "customPrompt": Ignore the /internal endpoints.,
  "manifest": null,
} satisfies AgentRunInputs

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AgentRunInputs
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


