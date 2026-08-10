
# AgentRun


## Properties

Name | Type
------------ | -------------
`id` | number
`agent` | number
`agentName` | string
`project` | number
`testPlan` | number
`testPlanRun` | number
`triggerType` | string
`triggeredBy` | number
`status` | string
`host` | string
`containerId` | string
`systemPromptVersion` | number
`promptVersion` | number
`imageTag` | string
`opencodeVersion` | string
`model` | string
`startedAt` | string
`endedAt` | string
`exitCode` | number
`error` | string
`artifactsUrl` | string
`rating` | number
`ratingReasons` | Array&lt;string&gt;
`ratingComment` | string
`ratedBy` | number
`ratedAt` | string
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { AgentRun } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "agent": 1,
  "agentName": Nightly API checks,
  "project": 1,
  "testPlan": 12,
  "testPlanRun": 34,
  "triggerType": assignment,
  "triggeredBy": 1,
  "status": running,
  "host": docker-local,
  "containerId": 3f2b9c1d8a04,
  "systemPromptVersion": 1,
  "promptVersion": 1,
  "imageTag": tc-agent-runner:0.1.0,
  "opencodeVersion": 0.4.2,
  "model": glm-5.2,
  "startedAt": 2026-08-05T17:11:24.000Z,
  "endedAt": 2026-08-05T17:18:02.000Z,
  "exitCode": 0,
  "error": null,
  "artifactsUrl": null,
  "rating": 4,
  "ratingReasons": null,
  "ratingComment": Took far longer than a manual pass would have.,
  "ratedBy": 1,
  "ratedAt": 2026-08-05T17:20:00.000Z,
  "createdAt": 2026-08-05T17:11:24.000Z,
  "updatedAt": 2026-08-05T17:11:24.000Z,
} satisfies AgentRun

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AgentRun
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


