
# Agent


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`type` | string
`description` | string
`enabled` | boolean
`customPrompt` | string
`config` | { [key: string]: string; }
`project` | number
`user` | number
`createdBy` | number
`updatedBy` | number
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { Agent } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "name": Nightly API checks,
  "type": api-testing-agent,
  "description": Runs contract checks against the staging API,
  "enabled": true,
  "customPrompt": Ignore the /internal endpoints.,
  "config": null,
  "project": 1,
  "user": 88,
  "createdBy": 1,
  "updatedBy": 1,
  "createdAt": 2026-08-05T17:11:24.000Z,
  "updatedAt": 2026-08-05T17:11:24.000Z,
} satisfies Agent

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Agent
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


