
# AgentPayload


## Properties

Name | Type
------------ | -------------
`name` | string
`type` | string
`description` | string
`enabled` | boolean
`customPrompt` | string
`config` | { [key: string]: string; }
`project` | number

## Example

```typescript
import type { AgentPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": Nightly API checks,
  "type": api-testing-agent,
  "description": Runs contract checks against the staging API,
  "enabled": true,
  "customPrompt": Ignore the /internal endpoints.,
  "config": null,
  "project": 1,
} satisfies AgentPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AgentPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


