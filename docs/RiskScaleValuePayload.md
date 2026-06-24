
# RiskScaleValuePayload


## Properties

Name | Type
------------ | -------------
`project` | number
`axis` | string
`name` | string
`score` | number
`color` | string
`position` | number

## Example

```typescript
import type { RiskScaleValuePayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "project": 1,
  "axis": likelihood,
  "name": Likely,
  "score": 4,
  "color": #f04438,
  "position": 4,
} satisfies RiskScaleValuePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RiskScaleValuePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


