
# SuiteNode


## Properties

Name | Type
------------ | -------------
`id` | number
`type` | string
`newNode` | number

## Example

```typescript
import type { SuiteNode } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "type": Suite,
  "newNode": 1,
} satisfies SuiteNode

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SuiteNode
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


