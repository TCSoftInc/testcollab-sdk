
# RiskBurndownItem


## Properties

Name | Type
------------ | -------------
`label` | string
`openExposure` | number
`plannedExposure` | number

## Example

```typescript
import type { RiskBurndownItem } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "label": S4,
  "openExposure": 80,
  "plannedExposure": 90,
} satisfies RiskBurndownItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RiskBurndownItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


