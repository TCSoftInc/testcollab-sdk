
# RiskStatusPayload


## Properties

Name | Type
------------ | -------------
`project` | number
`name` | string
`color` | string
`isClosed` | boolean
`position` | number

## Example

```typescript
import type { RiskStatusPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "project": 1,
  "name": Mitigating,
  "color": #2d6bcf,
  "isClosed": false,
  "position": 3,
} satisfies RiskStatusPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RiskStatusPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


