
# DefectsTimeline


## Properties

Name | Type
------------ | -------------
`seriesTime` | Array&lt;string&gt;
`defectsSeries` | Array&lt;number&gt;

## Example

```typescript
import type { DefectsTimeline } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "seriesTime": ["OCT 2018","JAN 2019","Nov 2019"],
  "defectsSeries": [1,5,3],
} satisfies DefectsTimeline

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DefectsTimeline
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


