
# LinkedtestcasePayload


## Properties

Name | Type
------------ | -------------
`issueKey` | string
`issueId` | number
`im` | string
`project` | number
`testcase` | number
`imProjectId` | string
`imInstanceId` | string

## Example

```typescript
import type { LinkedtestcasePayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "issueKey": TP1-1,
  "issueId": 1,
  "im": jira,
  "project": 1,
  "testcase": 1,
  "imProjectId": null,
  "imInstanceId": null,
} satisfies LinkedtestcasePayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as LinkedtestcasePayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


