
# ExecutionContext

TCV-6814. Where a non-manual result came from, recorded by the tool that reported it. This is what makes a result auditable rather than merely labelled — it answers \"which pipeline run produced this, using which tool version, against which build\".

## Properties

Name | Type
------------ | -------------
`tool` | string
`toolVersion` | string
`provider` | string
`runUrl` | string
`build` | number

## Example

```typescript
import type { ExecutionContext } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "tool": tc-cli,
  "toolVersion": 1.15.0,
  "provider": Azure DevOps,
  "runUrl": https://dev.azure.com/acme/web/_build/results?buildId=55,
  "build": 16,
} satisfies ExecutionContext

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ExecutionContext
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


