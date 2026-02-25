
# ReleaseReadinessConfigurationCoverage

Coverage breakdown for a single configuration. Shows execution statistics aggregated across all test plans in the release that use this configuration. 

## Properties

Name | Type
------------ | -------------
`configurationId` | number
`parameters` | { [key: string]: string; }
`testPlanId` | number
`testPlanTitle` | string
`total` | number
`executed` | number
`passed` | number
`failed` | number
`passRate` | number

## Example

```typescript
import type { ReleaseReadinessConfigurationCoverage } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "configurationId": 12,
  "parameters": {"browser":"Chrome","os":"Windows"},
  "testPlanId": 5,
  "testPlanTitle": Smoke Test Plan,
  "total": 100,
  "executed": 85,
  "passed": 75,
  "failed": 5,
  "passRate": 88.2,
} satisfies ReleaseReadinessConfigurationCoverage

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReleaseReadinessConfigurationCoverage
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


