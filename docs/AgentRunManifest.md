
# AgentRunManifest

Run manifest written to /agent/run.json. Tells the container which project, plan and plan run it is working on, which type it is, and which prompt and image versions produced it. 

## Properties

Name | Type
------------ | -------------
`project` | number
`testPlan` | number
`testPlanRun` | number
`agent` | number
`agentType` | string
`runtime` | string
`fields` | { [key: string]: string; }
`systemPromptVersion` | number
`promptVersion` | number
`imageTag` | string

## Example

```typescript
import type { AgentRunManifest } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "project": 1,
  "testPlan": 12,
  "testPlanRun": 34,
  "agent": 1,
  "agentType": dummy-agent,
  "runtime": direct,
  "fields": null,
  "systemPromptVersion": 1,
  "promptVersion": 1,
  "imageTag": tc-agent-runner:latest,
} satisfies AgentRunManifest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AgentRunManifest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


