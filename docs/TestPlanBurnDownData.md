
# TestPlanBurnDownData


## Properties

Name | Type
------------ | -------------
`startDate` | string
`dueDate` | string
`totalCases` | number
`dayLabels` | Array&lt;string&gt;
`idealWorkloadSeries` | Array&lt;number&gt;
`timelineSeries` | Array&lt;string&gt;
`workDoneSeries` | Array&lt;number&gt;
`workLeftSeries` | Array&lt;number&gt;

## Example

```typescript
import type { TestPlanBurnDownData } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "startDate": 2019-06-11T17:11:24.000Z,
  "dueDate": 2019-06-20T17:11:24.000Z,
  "totalCases": 10,
  "dayLabels": [1,2,3,4,5,6,7,8,9,10],
  "idealWorkloadSeries": [110,100,90,80,70,60,50,40,30,20,10,0],
  "timelineSeries": ["2019-06-11T00:00:00.000Z","2019-06-12T00:00:00.000Z","2019-06-13T00:00:00.000Z","2019-06-14T00:00:00.000Z","2019-06-15T00:00:00.000Z","2019-06-16T00:00:00.000Z","2019-06-17T00:00:00.000Z","2019-06-18T00:00:00.000Z","2019-06-19T00:00:00.000Z","2019-06-20T00:00:00.000Z"],
  "workDoneSeries": [100,110,125,95,64,76,62,44,35,29,18,2],
  "workLeftSeries": [1,0,1,0,1,0,1,0,1,0,0,0],
} satisfies TestPlanBurnDownData

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanBurnDownData
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


