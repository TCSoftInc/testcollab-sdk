
# AgentType


## Properties

Name | Type
------------ | -------------
`slug` | string
`label` | string
`description` | string
`group` | string
`icon` | string
`assignable` | boolean
`config` | [Array&lt;AgentTypeConfigInput&gt;](AgentTypeConfigInput.md)

## Example

```typescript
import type { AgentType } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "slug": dummy-agent,
  "label": Dummy Agent (dev),
  "description": Does nothing. Exists to exercise the agent plumbing in development.,
  "group": specialist,
  "icon": experiment,
  "assignable": true,
  "config": null,
} satisfies AgentType

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AgentType
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


