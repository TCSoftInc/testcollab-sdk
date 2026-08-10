
# AgentRunRatingPayload


## Properties

Name | Type
------------ | -------------
`rating` | number
`ratingReasons` | Array&lt;string&gt;
`ratingComment` | string

## Example

```typescript
import type { AgentRunRatingPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "rating": 4,
  "ratingReasons": null,
  "ratingComment": Took far longer than a manual pass would have.,
} satisfies AgentRunRatingPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AgentRunRatingPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


