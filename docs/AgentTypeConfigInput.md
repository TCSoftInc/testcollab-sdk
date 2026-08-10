
# AgentTypeConfigInput


## Properties

Name | Type
------------ | -------------
`name` | string
`label` | string
`type` | string
`required` | boolean
`help` | string
`defaultValue` | string
`entity` | string
`multiple` | boolean
`options` | [Array&lt;AgentTypeConfigInputOption&gt;](AgentTypeConfigInputOption.md)

## Example

```typescript
import type { AgentTypeConfigInput } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": echo_message,
  "label": Echo message,
  "type": text,
  "required": true,
  "help": Written to the run log and nowhere else.,
  "defaultValue": hello,
  "entity": suite,
  "multiple": false,
  "options": null,
} satisfies AgentTypeConfigInput

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AgentTypeConfigInput
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


