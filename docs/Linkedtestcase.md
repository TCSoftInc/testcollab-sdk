
# Linkedtestcase


## Properties

Name | Type
------------ | -------------
`issueKey` | string
`im` | string
`project` | [Project](Project.md)
`testcase` | [TestCase](TestCase.md)
`createdBy` | [User](User.md)
`createdAt` | string

## Example

```typescript
import type { Linkedtestcase } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "issueKey": TestCase,
  "im": Issue Manager string,
  "project": null,
  "testcase": null,
  "createdBy": null,
  "createdAt": 2019-04-30T17:11:24.000Z,
} satisfies Linkedtestcase

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Linkedtestcase
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


